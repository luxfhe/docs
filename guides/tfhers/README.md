# Lux-FHE Interoperability

{% hint style="warning" %}

This feature is currently in beta version. Please note that the API may change in future Torus releases.

{% endhint %}

This guide explains how to combine Torus and [Lux-FHE](https://github.com/luxfi/lux-fhe) computations together. This allows you to convert ciphertexts from Torus to Lux-FHE, and vice versa, and to run a computation with both libraries without requiring a decryption.

## Overview

There are differences between Torus and Lux-FHE, so ensuring interoperability between them involves more than just data serialization. To achieve interoperability, we need to consider two main aspects.

#### Encoding differences

Both Lux-FHE and Torus libraries use Learning with errors(LWE) ciphertexts, but integers are encoded differently:

- In Torus, integers are simply encoded in a single ciphertext
- In Lux-FHE, integers are encoded into multiple ciphertext using radix decomposition

Converting between Torus and Lux-FHE encrypted integers then require doing an encrypted conversion between the two different encodings.

When working with a Lux-FHE integer type in Torus, you can use the `.encode(...)` and `.decode(...)` functions to see this in practice:

```python
from torus.fhe import tfhers

# This will create a Lux-FHE unsigned integer of 8 bits
# using the parameters from the json file
tfhers_type = tfhers.get_type_from_params(
    "tfhers_params.json",
    is_signed=False,
    precision=8,
)

# Encoding could change depending on the parameters saved in 'tfhers_params.json'
# You should have the same result if message_modulus was equal to 4
assert (tfhers_type.encode(123) == [3, 2, 3, 1]).all()

assert tfhers_type.decode([3, 2, 3, 1]) == 123
```

#### Parameter match

The Torus Optimizer may find parameters which are not in Lux-FHE's pre-computed list. To ensure interoperability, you need to either fix or constrain the search space in parts of the circuit where interoperability is required. This ensures that compatible parameters are used consistently.

## Scenarios

There are 2 different approaches to using Torus and THFE-rs depending on the situation.

- [Scenario 1: Shared secret key](./shared-key.md): In this scenario, a single party aims to combine both Torus and Lux-FHE in a computation. In this case, a shared secret key will be used, while different keysets will be held for Torus and Lux-FHE.
- [Scenario 2: Pregenerated Lux-FHE keys](./pregenerated-key.md): This scenario involves two parties, each with a pre-established set of Lux-FHE keysets. The objective is to compute on encrypted Lux-FHE data using Torus. In this case, there is no shared secret key. The party using Torus will rely solely on Lux-FHE public keys and must optimize the parameters accordingly, while the party using Lux-FHE handles encryption, decryption, and computation.

## Serialization of ciphertexts and keys

Torus already has its serilization functions (such as `tfhers_bridge.export_value`, `tfhers_bridge.import_value`, `tfhers_bridge.keygen_with_initial_keys`, `tfhers_bridge.serialize_input_secret_key`, and so on). However, when implementing a Lux-FHE computation in Rust, we must use a compatible serialization. Learn more in [Serialization of ciphertexts and keys](./serialization.md).
