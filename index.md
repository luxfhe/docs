---
layout: default
title: Lux FHE Documentation
---

# Lux FHE Documentation

**Fully Homomorphic Encryption for Everyone**

## Quick Start

```python
from luxfhe import Client, Server

client = Client()
encrypted = client.encrypt(42)

server = Server(client.evaluation_key)
result = server.add(encrypted, client.encrypt(8))

print(client.decrypt(result))  # 50
```

## Documentation Sections

- [Getting Started](./get-started/) - Installation and first steps
- [Core Features](./core-features/) - FHE operations
- [Guides](./guides/) - How-to guides  
- [Torus ML](./ml/) - Machine learning on encrypted data
- [fhEVM](./fhevm/) - FHE for blockchain
- [Resources](./resources) - Curated links

## Related

- [Examples](https://github.com/luxfhe/examples)
- [Handbook](https://github.com/luxfhe/handbook)
- [Workshop](https://github.com/luxfhe/workshop)
