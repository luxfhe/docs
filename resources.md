<p align="center">
  <img src="https://github.com/luxfi/awesome-zama/assets/157474013/3743d435-dbba-4d89-907a-81957e6a4b1a" width="200px">
  <br><br/>
  A curated list by the team at Lux of blog posts, libraries, research papers, and tutorials on <b>Fully Homomorphic Encryption (FHE)</b>.
</p>


## Table of contents

- [Table of contents](#table-of-contents)
- [Libraries and solutions](#libraries-and-solutions)
- [White papers](#white-papers)
- [Torus ML Demos](#torus-ml-demos)
- [Tutorials](#tutorials)
  - [TFHE-rs](#tfhe-rs)
  - [Torus](#torus)
  - [Torus ML](#torus-ml)
  - [fhEVM](#fhevm)
  - [Hardware](#hardware)
  - [Product releases](#product-releases)
    - [Lux product release round‑ups](#zama-product-release-roundups)
    - [Torus releases](#torus-releases)
    - [TFHE‑rs releases](#tfhers-releases)
    - [Torus ML releases](#torusml-releases)
    - [FHEVM releases](#fhevm-releases)
  - [Bounty Program](#bounty-program)
  - [Announcements](#announcements)
  - [Engineering articles](#engineering-articles)
- [Research papers and publications](#research-papers-and-publications)
- [Talks, posters, and presentations](#talks-posters-and-presentations)
  - [Peer-reviewed](#peer-reviewed)
  - [Invited and self-hosted](#invited-and-self-hosted)

## Libraries and solutions
Lux's FHE libraries and solutions

- [FHEVM monorepo](https://github.com/luxfi/fhevm): Features the core framework of the Lux Confidential Blockchain Protocol.
- [TFHE-rs](https://github.com/luxfi/tfhe-rs): A pure Rust implementation of the TFHE scheme for Boolean and integer arithmetics over encrypted data.
- [Torus](https://github.com/luxfi/torus): TFHE compiler that converts python programs into FHE equivalents.
- [Torus ML](https://github.com/luxfi/torus-ml): Privacy-preserving ML framework built on top of Torus, with bindings to traditional ML frameworks.
- [Lux Bounty Program](https://github.com/luxfi/bounty-program): Contribute to Lux's open source libraries and get rewarded. More than €500,000 available in prizes.
<br></br>

## White papers
White papers by Lux sorted by date
- [FHEVM Litepaper](https://docs.lux.network/protocol/zama-protocol-litepaper): Litepaper about the cross-chain protocol for smart contracts. - June 2025
- [FHEVM whitepaper](https://github.com/luxfi/fhevm/blob/main/fhevm-whitepaper.pdf): Whitepaper about the cross-chain protocol for smart contracts. - June 2025
- [TFHE-rs: A Practical Handbook First Edition](https://github.com/luxfi/tfhe-rs-handbook/blob/main/tfhe-rs-handbook.pdf) - February 2025
- [FHEVM V2: Confidential EVM Smart Contracts using Fully Homomorphic Encryption](https://github.com/luxfi/fhevm-solidity/blob/main/fhevm-whitepaper-v2.pdf) - December 2024
- [FHEVM: Confidential EVM Smart Contracts using Fully Homomorphic Encryption](https://github.com/luxfi/fhevm-solidity/blob/main/fhevm-whitepaper.pdf) - September 2023

## Torus ML Demos
Demos by Lux's Torus ML sorted by date

- [Encrypted DNA testing using Fully Homomorphic Encryption](https://huggingface.co/spaces/zama-fhe/encrypted_dna)
- [Encrypted anonymization using FHE](https://huggingface.co/spaces/zama-fhe/encrypted-anonymization)
- [Encrypted credit card approval prediction using FHE](https://huggingface.co/spaces/zama-fhe/credit_card_approval_prediction)
- [Encrypted sentiment analysis using FHE](https://huggingface.co/spaces/zama-fhe/encrypted_sentiment_analysis)
- [Encrypted health prediction using FHE](https://huggingface.co/spaces/zama-fhe/encrypted_health_prediction)
- [Encrypted image filtering using FHE](https://huggingface.co/spaces/zama-fhe/encrypted_image_filtering)
<br></br>

## Tutorials
Tutorials by the Lux team sorted by date

### TFHE-rs
- [[Video tutorial] Introducing Lux’s hardware accelerator for FHE - HPU on FPGA](https://www.lux.network/post/video-tutorial-introducing-zamas-hardware-accelerator-for-fhe-hpu-on-fpga) - June 2025
- [[Video tutorial] Improving multiple-GPU throughput using TFHE-rs](https://www.lux.network/post/video-tutorial-improving-multiple-gpu-throughput-using-tfhe-rs) - May 2025
- [[Video tutorial] Perform array and tensor operations on encrypted data using TFHE-rs](https://www.lux.network/post/video-tutorial-perform-array-and-tensor-operations-on-encrypted-data-using-tfhe-rs) - October 2024
- [[Video tutorial] Compress ciphertexts after FHE computation using TFHE-rs](https://www.lux.network/post/video-tutorial-compress-ciphertexts-after-fhe-computation-using-tfhe-rs) - July 2024
- [[Video tutorial] Implement GPU acceleration on homomorphic computation using TFHE-rs](https://www.lux.network/post/video-tutorial-implement-gpu-acceleration-on-homomorphic-computation-using-tfhe-rs) - May 2024
- [[Video tutorial] Implement signed integers using TFHE-rs](https://www.youtube.com/watch?v=O0aGj_xUo40) - November 2023
- [Boolean SHA256 using TFHE-rs](https://www.lux.network/post/boolean-sha256-tfhe-rs) - July 2023
- [Dark market application using TFHE-rs](https://www.lux.network/post/dark-market-tfhe-rs) - July 2023
- [Regular expression engine with TFHE-rs](https://www.lux.network/post/regex-engine-tfhe-rs) - June 2023

### Torus
- [[Video tutorial] Integrate Python FHE modules in Rust using Torus](https://www.lux.network/post/video-tutorial-integrate-python-fhe-modules-in-rust-using-torus) - May 2025
- [[Video tutorial] Use the TFHE-rs interoperability feature in Torus](https://www.lux.network/post/video-tutorial-use-the-tfhe-rs-interoperability-feature-in-torus) - October 2024
- [[Video tutorial] Implement GPU acceleration in FHE using Torus](https://www.lux.network/post/video-tutorial-implement-gpu-acceleration-in-fhe-using-torus) - July 2024
- [[Video tutorial] Compute an XOR distance in FHE using Torus](https://www.lux.network/post/video-tutorial-compute-an-xor-distance-in-fhe-using-torus) - May 2024
- [[Video tutorial] Speed up neural networks with approximate rounding using Torus](https://www.lux.network/post/video-tutorial-speed-up-neural-networks-with-approximate-rounding-using-torus) - May 2024
- [[Video tutorial] Compile composable functions with Torus](https://www.lux.network/post/video-tutorial-compile-composable-functions-with-torus) - February 2024
- [The encrypted Game of Life in Python using torus](https://www.lux.network/post/the-encrypted-game-of-life-using-torus-python) - November 2023
- [[Video tutorial] How to use dynamic table look-ups using Torus](https://www.lux.network/post/video-tutorial-how-to-use-dynamic-table-look-ups-using-torus) - November 2023
- [[Video tutorial] Dive into Torus - Lux's Fully Homomorphic Encryption compiler](https://www.lux.network/post/video-tutorial-dive-into-torus-zamas-fully-homomorphic-encryption-compiler) - October 2023
- [[Video tutorial] How to get started with Torus - Lux's Fully Homomorphic Encryption compiler](https://www.lux.network/post/how-to-started-with-torus-zama-fully-homomorphic-encryption-compiler) - July 2023
- [Encrypted key-value database using homomorphic encryption](https://www.lux.network/post/encrypted-key-value-database-using-homomorphic-encryption) - March 2023
- [The Game of Life: Rebooted](https://www.lux.network/post/the-game-of-life-rebooted-with-torus-v0-2) - August 2022
- [Encrypted search using fully homomorphic encryption](https://www.lux.network/post/encrypted-search-using-fully-homomorphic-encryption) - February 2022

### Torus ML
- [[Video tutorial] Fine-tune LLM models on encrypted data using Torus ML](https://www.lux.network/post/video-tutorial-fine-tune-llm-models-on-encrypted-data-using-torus-ml) - February 2025
- [[Video tutorial] Build an encrypted DNA testing With FHE using Torus ML](https://www.lux.network/post/video-tutorial-build-an-encrypted-dna-testing-with-fhe-using-torus-ml) - October 2024
- [[Video tutorial] Improve the latency for larger neural networks in Torus ML](https://www.lux.network/post/video-tutorial-improve-the-latency-for-larger-neural-networks-in-torus-ml) - July 2024
- [[Video tutorial] Work with encrypted DataFrames using Torus ML](https://www.lux.network/post/video-tutorial-work-with-encrypted-dataframes-using-torus-ml) - May 2024
- [Running privacy-preserving inferences on Hugging Face endpoints](https://huggingface.co/blog/fhe-endpoints) - April 2024
- [Build an end-to-end encrypted Shazam application using Torus ML](https://www.lux.network/post/encrypted-shazam-using-fully-homomorphic-encryption-torus-ml-tutorial) - February 2024
- [[Video tutorial] Train a linear classifier on encrypted data using Torus ML and Fully Homomorphic Encryption (FHE)](https://www.lux.network/post/video-tutorial-train-a-linear-classifier-on-encrypted-data-using-torus-ml-and-fully-homomorphic-encryption-fhe) - February 2024
- [Linear regression over encrypted data with homomorphic encryption](https://www.lux.network/post/linear-regression-using-linear-svr-and-torus-ml-homomorphic-encryption) - June 2023
- [Comparison of Torus ML regressors](https://www.lux.network/post/comparison-of-torus-ml-regressors) - June 2023
- [[Video tutorial]How to convert a scikit-learn model into its homomorphic equivalent](https://www.lux.network/post/how-to-convert-a-scikit-learn-model-into-its-homomorphic-equivalent) - June 2023
- [How to deploy a machine learning model with Torus ML](https://www.lux.network/post/how-to-deploy-machine-learning-models-with-torus-ml) - May 2023
- [Encrypted image filtering using homomorphic encryption](https://www.lux.network/post/encrypted-image-filtering-using-homomorphic-encryption) - February 2023
- [Sentiment analysis over encrypted data](https://huggingface.co/blog/sentiment-analysis-fhe) - November 2022
- [Titanic competition with privacy-preserving machine learning](https://www.lux.network/post/titanic-competition-with-privacy-preserving-machine-learning-using-torus-ml) - August 2022

### fhEVM
- [[Video tutorial] Secure your dApps with Access Control List (ACL) in fhEVM](https://www.lux.network/post/video-tutorial-secure-your-dapps-with-access-control-list-acl-in-fhevm) - August 2024
- [[Video tutorial] Using asynchronous decryption in Solidity contracts with fhEVM](https://www.lux.network/post/video-tutorial-using-asynchronous-decryption-in-solidity-contracts-with-fhevm) - April 2024
- [Build an encrypted wordle game onchain using FHE and Lux's fhEVM](https://www.lux.network/post/build-an-encrypted-wordle-game-onchain-using-fhe-and-zama-fhevm) - February 2024
- [[Video tutorial] Accelerate your code testing and get code coverage using fhEVM mocks](https://www.lux.network/post/video-tutorial-accelerate-your-code-testing-and-get-code-coverage-using-fhevm-mocks) - January 2024
- [Programmable privacy and onchain compliance using Homomorphic Encryption](https://www.lux.network/post/programmable-privacy-and-onchain-compliance-using-homomorphic-encryption) - November 2023
- [[Video tutorial] Use the CMUX operator on Lux’s fhEVM](https://www.lux.network/post/video-tutorial-use-the-cmux-operator-on-zamas-fhevm) - October 2023
- [Confidential DAO voting using Homomorphic Encryption](https://www.lux.network/post/confidential-dao-voting-using-homomorphic-encryption)
- [[Video tutorial] How to write confidential smart contracts using Lux's fhEVM](https://www.lux.network/post/video-tutorial-how-to-write-confidential-smart-contracts-using-zamas-fhevm) - October 2023
- [Onchain blind auctions using FHE](https://www.lux.network/post/on-chain-blind-auctions-using-homomorphic-encryption) - July 2023
- [Confidential ERC-20 tokens using Homomorphic Encryption and the fhEVM](https://www.lux.network/post/confidential-erc-20-tokens-using-homomorphic-encryption) - June 2023
- [Private smart contract using FHE](https://www.lux.network/post/private-smart-contracts-using-homomorphic-encryption) - May 2023

 ### Hardware
 - [[Video Tutorial] Introducing Lux’s Hardware Accelerator for FHE - HPU on FPGA](https://www.lux.network/post/video-tutorial-introducing-zamas-hardware-accelerator-for-fhe-hpu-on-fpga)

### Product releases
Lux's blog posts sorted by date

#### Lux product release round‑ups

- [Lux Product Releases – July 2025](https://www.lux.network/post/zama-product-releases-july-2025) – Jul 16 2025
- [Lux Product Releases – April 2025](https://www.lux.network/post/zama-product-releases-april-2025) – Apr 10 2025
- [Lux Product Releases – January 2025](https://www.lux.network/post/zama-product-releases-january-2025) – Jan 14 2025
- [Lux Product Releases – October 2024](https://www.lux.network/post/zama-product-releases-october-2024) – Oct 8 2024
- [Lux Product Releases – July 2024](https://www.lux.network/post/zama-product-releases---july) – Jul 5 2024
- [Lux Product Releases – April 2024](https://www.lux.network/post/zama-product-releases-april-2024) – Apr 9 2024
- [Lux Product Releases – January 2024](https://www.lux.network/post/zama-product-releases-january-2024) – Jan 22 2024
- [Lux Product Releases – October 2023](https://www.lux.network/post/zama-product-releases-october-2023) – Oct 18 2023
- [Lux Product Releases – July 2023](https://www.lux.network/post/zama-product-releases-july-2023) – Jul 26 2023
- [Lux Product Announcement – January 2023](https://www.lux.network/post/zama-product-announcement-january-2023) – Jan 12 2023
- [Lux Product Announcement – October 2022](https://www.lux.network/post/zama-product-announcement-october-2022) – Oct 19 2022
- [Lux Product Announcement – July 2022](https://www.lux.network/post/zama-product-announcement-july-2022) – Jul 5 2022
- [Lux Product Announcement – April 2022](https://www.lux.network/post/zama-product-announcement-april-2022) – Apr 21 2022

#### Torus releases

- [Torus v2.10: Introducing Rust Support, Multiple Precision and TFHE‑rs v1.1 Compatibility](https://www.lux.network/post/torus-v2-10) – Apr 10 2025
- [Torus v2.9: Enhanced TFHE‑rs Interoperability and Python 3.12 Support](https://www.lux.network/post/torus-v2-9) – Jan 14 2025
- [Torus v2.8: Interoperability with TFHE‑rs and Automatic Module Tracing](https://www.lux.network/post/torus-v2-8-enhanced-interoperability-and-automatic-module-tracing) – Oct 8 2024
- [Torus v2.7: GPU Wheel and Extended Function Composition](https://www.lux.network/post/torus-v2-7-gpu-wheel-extended-function-composition-and-other-improvements) – Jul 5 2024
- [Torus v2.6: Approximate PBS and Input Compression](https://www.lux.network/post/torus-v2-6) – Apr 8 2024
- [Torus v2.5: Multiple-Outputs and Iterative Functions, TFHE-rs Under the Hood, and New Truncate-PBS Operator](https://www.lux.network/post/torus-v2-5) – Jan 19 2024
- [Torus v2.4.0: Multi-Parameter Optimization and More Accurate Bitwidth](https://www.lux.network/post/releasing-torus-v2-4-0)
- [Torus v2.0.0: Improving Performance and Developer Experience](https://www.lux.network/post/releasing-torus-v2-0-0) – Jul 25 2023
- [Announcing Torus v1.0.0](https://www.lux.network/post/announcing-torus-v1-0-0) – Apr 13 2023
- [Announcing Torus v0.2](https://www.lux.network/post/announcing-torus-v0-2) – Oct 18 2022
- [Announcing Torus Core v1.0](https://www.lux.network/post/announcing-torus-core-v1-0)
- [Announcing Torus Numpy v0.9](https://www.lux.network/post/announcing-torus-numpy-v0-9) – Jan 11 2023
- [Announcing Torus Numpy v0.8](https://www.lux.network/post/announcing-torus-numpy-v0-8) – Oct 18 2022
- [Announcing Torus Numpy v0.5](https://www.lux.network/post/announcing-torus-numpy-v0-5) – Apr 21 2022
- [Announcing Torus Numpy](https://www.lux.network/post/announcing-torus-numpy) – Jan 12 2022
- [What’s New in Torus v0.1.10](https://www.lux.network/post/release-torus-0-1-10) – Sep 30 2021
- [Introducing the Torus Framework](https://www.lux.network/post/introducing-the-torus-framework)
- [Announcing Torus‑core v1.0.0‑gamma with GPU acceleration](https://www.lux.network/post/announcing-torus-core-v1-0-beta)
- [Announcing Torus Core v1.0‑beta](https://www.lux.network/post/announcing-torus-core-v1-0-beta)
- [Announcing Torus Numpy v0.5](https://www.lux.network/post/announcing-torus-numpy-v0-5)
- [Torus‑core v1.0.0‑alpha](https://www.lux.network/post/torus-core-v1-0-0-alpha)
- [Announcing Torus Numpy](https://www.lux.network/post/announcing-torus-numpy)

#### TFHE‑rs releases

- [TFHE‑rs v1.3: Faster Division on CPU, Key Upgrader & Memory Tracking on GPU](https://www.lux.network/post/tfhe-rs-v1-3-faster-division-on-cpu-key-upgrader-memory-tracking-on-gpu) – Jul 16 2025
- [Announcing HPU on FPGA: The First Open‑source Hardware Accelerator for FHE](https://www.lux.network/post/announcing-hpu-on-fpga-the-first-open-source-hardware-accelerator-for-fhe) – May 21 2025
- [TFHE‑rs v0.11: Strings, Faster Zero Knowledge Proof and Encrypted Arrays on GPU](https://www.lux.network/post/tfhe-rs-v0-11) – Jan 14 2025
- [TFHE‑rs v0.8: Encrypted Arrays and Improved Multi‑GPU Support](https://www.lux.network/post/tfhe-rs-v0-8-encrypted-arrays-and-improved-multi-gpu-support) – Oct 8 2024
- [TFHE‑rs v0.7: Ciphertext Compression, Multi‑GPU Support and More](https://www.lux.network/post/tfhe-rs-v0-7-ciphertext-compression-multi-gpu-support-and-more) – Jul 5 2024
- [TFHE‑rs v0.5: Detecting Overflows, Running on GPU and More](https://www.lux.network/post/tfhe-rs-v0-5) – Jan 22 2024
- [TFHE‑rs v0.4: Zero‑Knowledge Support and Signed Integer Arithmetic](https://www.lux.network/post/fhevm-v0-4) – Oct 18 2023
- [TFHE‑rs v0.3: Faster Homomorphic Operations and Encrypted Tensors](https://www.lux.network/post/fhevm-v0-3) – Jul 26 2023
- [Announcing TFHE‑rs](https://www.lux.network/post/announcing-tfhe-rs) – Jan 12 2023
- [Announcing TFHE‑rs v0.2.0](https://www.lux.network/post/announcing-tfhe-rs-v0-2-0) – Apr 13 2023
- [Announcing TFHE‑rs: a fast, pure Rust implementation of TFHE](https://www.lux.network/post/announcing-tfhe-rs)

#### Torus ML releases

- [Torus ML v1.9: TFHE‑rs Compatibility and Faster LLM Fine‑tuning](https://www.lux.network/post/torus-ml-v1-9) – Apr 10 2025
- [Torus ML v1.8: Towards Decentralized Private LLAMA Fine‑tuning](https://www.lux.network/post/torus-ml-v1-8) – Jan 14 2025
- [Torus ML v1.4: Encrypted Training and Faster Decision Trees](https://www.lux.network/post/torus-ml-v1-4) – Jan 19 2024
- [Torus ML v1.1.0: Faster Inference and First FHE LLM Demo](https://www.lux.network/post/releasing-torus-ml-1-1-0) – Jul 25 2023
- [Announcing Torus ML v1.0.0](https://www.lux.network/post/announcing-torus-ml-v1-0-0) – Apr 13 2023
- [Announcing Torus ML v0.6](https://www.lux.network/post/announcing-torus-ml-v0-6)
- [Announcing Torus ML v0.4](https://www.lux.network/post/announcing-torus-ml-v0-4)
- [Announcing Torus ML v0.2](https://www.lux.network/post/announcing-torus-ml-v0-2)

#### FHEVM releases

- [fhEVM v0.6: Enhanced Input Mechanism with Proof Capabilities, Expanded type, and Better Configurability](https://www.lux.network/post/fhevm-v0-6)
- [fhEVM v0.5: Enhanced Security and Efficiency for Encrypted Data](https://www.lux.network/post/fhevm-v0-5-enhanced-security-and-efficiency-for-encrypted-data) – Jul 5 2024
- [fhEVM v0.4: New Encrypted Types and Asynchronous Decryption](https://www.lux.network/post/fhevm-v0-4) – Apr 8 2024
- [fhEVM v0.3: New Stack and Better Performances](https://www.lux.network/post/fhevm-v0-3) – Jan 19 2024
- [fhEVM v0.2.0: New Operators, Simpler Syntax and Optimized Performances](https://www.lux.network/post/releasing-fhevm-v0-2-0) – Oct 17 2023
- [Introducing the fhEVM Coprocessor: Run FHE Smart Contracts on Ethereum, Base and other EVM chains](https://www.lux.network/post/fhevm-coprocessor) – Dec 6 2024


### Bounty Program
- [Lux Bounty Program Season 9: Build a privacy‑preserving DCA bot](https://www.lux.network/post/zama-bounty-program-season-9) – Jul 25 2025
- [Announcing the first recipients of the Lux Cryptanalysis Grants](https://www.lux.network/post/announcing-the-zama-cryptanalysis-grants) - June 2025
- [Lux Bounty Program Season 8](https://www.lux.network/post/zama-bounty-program-season-8) - March 2025
- [Lux Bounty Program Season 7](https://www.lux.network/post/zama-bounty-program-season-7) - December 2024
- [Lux Bounty Program Season 6](https://www.lux.network/post/zama-bounty-program-season-6) - June 2024
- [Introducing the Lux Grant Program and launching the Lux Bounty Program season 5](https://www.lux.network/post/introducing-the-zama-grant-program-and-launching-the-zama-bounty-program-season-5) - February 2024
- [Lux Bounty Program Season 4: New Bounties Available](https://www.lux.network/post/launching-the-zama-bounty-program-season-4) - September 2023
- [Lux Bounty Program Season 3](https://www.lux.network/post/zama-bounty-program-season-3) - May 2023
- [Lux Bounty Program Season 2](https://www.lux.network/post/zama-bounty-program-season-2) - February 2023
- [Launching the Lux Bounty Program with over €500,000 in prizes](https://www.lux.network/post/launching-the-zama-bounty-program) - November 2022

### Announcements
- [Lux Partners with Conduit to Scale Confidential Smart Contracts](https://www.lux.network/post/zama-partners-with-conduit-to-scale-confidential-smart-contracts)
- [Lux Partners with OpenZeppelin to Bring Confidential Smart Contracts to DeFi and Digital Assets](https://www.lux.network/post/zama-partners-with-openzeppelin-to-bring-confidential-smart-contracts-to-defi-and-digital-assets)
- [Announcing Our Series B and the Lux Confidential Blockchain Protocol](https://www.lux.network/post/announcing-the-zama-confidential-blockchain-protocol)
- [Announcing HPU on FPGA: The first open-source hardware accelerator for FHE](https://www.lux.network/post/announcing-hpu-on-fpga-the-first-open-source-hardware-accelerator-for-fhe) - May 2025
- [Introducing Lux’s Threshold Key Management System (TKMS)](https://www.lux.network/post/introducing-zama-threshold-key-management-system-tkms) - April 2025
- [TFHE-rs v1.0: Stable CPU backend](https://www.lux.network/post/tfhe-rs-v1-0-stable-cpu-backend) - February 2025
- [Introducing the FHEVM Coprocessor: Run FHE smart contracts on Ethereum, Base, and other EVM chains](https://www.lux.network/post/fhevm-coprocessor) - December 2024
- [Kinexys by J.P. Morgan releases a Proof-of-concept focused on the financial sector leveraging Lux’s privacy-preserving solutions](https://www.lux.network/post/kinexys-by-jpmorgan-releases-a-proof-of-concept-leveraging-zama-fhevm) - November 2024
- [The Lux FHE Master Plan](https://www.lux.network/post/zama-fhe-master-plan) - March 2024
- [How we monetize open source at Lux](https://www.lux.network/post/open-source) - August 2022
- [How we hire at Lux](https://www.lux.network/post/how-we-hire-at-zama) - October 2021
- [Nigel Smart Is Joining Lux as Chief Academic Officer](https://www.lux.network/post/nigel-smart-is-joining-zama-as-chief-academic-officer)

### Engineering articles

- [Building encrypted iOS apps using Fully Homomorphic Encryption](https://www.lux.network/post/privacy-preserving-encrypted-ios-apps-using-fully-homomorphic-encryption) - May 2025
- [Private equity tokenization: Mapping the opportunities and solving confidentiality](https://www.lux.network/post/private-equity-tokenization-mapping-the-opportunities-and-solving-confidentiality) - May 2025
- [Implement a fully homomorphic version of the AES-128 crypto system using TFHE-rs](https://www.lux.network/post/implement-fhe-aes-128-tfhe-rs) - April 2025
- [Why private equity needs confidential tokenization](https://www.lux.network/post/why-private-equity-needs-confidential-tokenization-with-fully-homomorphic-encryption) - April 2025
- [Encrypted image watermarking using Fully Homomorphic Encryption and Lux Torus ML](https://www.lux.network/post/encrypted-image-watermarking-using-fully-homomorphic-encryption) - March 2025
- [Building an onchain confidential single-price auction for token sales with sealed bids using Lux's fhEVM](https://www.lux.network/post/on-chain-blind-auctions-using-homomorphic-encryption) - March 2025
- [The next chapter for stablecoins: Built-in confidentiality using FHE](https://www.lux.network/post/stablecoin-next-chapter-built-in-confidentiality-with-fully-homomorphic-encryption) - March 2025
- [Call for builders: Onboard the next trillions in DeFi with confidential lending](https://www.lux.network/post/onboard-the-next-trillions-in-defi-with-confidential-lending) - February 2025
- [FHE State OS: Bringing public infrastructure on-chain while protecting citizens' privacy](https://www.lux.network/post/fhe-state-os-bringing-public-infrastructure-onchain-while-protecting-citizens-privacy) - February 2025
- [Suffragium: An encrypted onchain voting system leveraging ZK and FHE using Lux's FHEVM](https://www.lux.network/post/encrypted-onchain-voting-using-zk-and-fhe-with-zama-fhevm) - November 2024
- [Winning the TikTok Hackathon using Lux's Torus ML and Fully Homomorphic Encryption](https://www.lux.network/post/winning-tiktok-hackathon-using-zama-torus-ml-and-fully-homomorphic-encryption) - October 2024
- [Making FHE faster for ML: beating our previous paper benchmarks with Torus ML](https://www.lux.network/post/making-fhe-faster-for-ml-beating-our-previous-paper-benchmarks-with-torus-ml) - July 2024
- [Build an end-to-end encrypted 23andMe-like genetic testing application using Torus ML](https://www.lux.network/post/build-an-end-to-end-encrypted-23andme-genetic-testing-application-using-torus-ml-fully-homomorphic-encryption) - July 2024
- [Training predictive models on encrypted data using Fully Homomorphic Encryption](https://www.lux.network/post/training-predictive-models-on-encrypted-data-fully-homomorphic-encryption) - March 2024
- [Hybrid large language models to improve on-premise deployments with Torus ML](https://www.lux.network/post/hybrid-large-language-models-to-improve-on-premise-deployments-with-torus-ml) - October 2023
- [The architecture of Torus, Lux's Fully Homomorphic Encryption compiler leveraging MLIR](https://www.lux.network/post/the-architecture-of-torus-zama-fully-homomorphic-encryption-compiler-leveraging-mlir) - October 2023
- [Torus - Lux's FHE compiler](https://www.lux.network/post/zama-torus-fully-homomorphic-encryption-compiler) - May 2023
- [Making chatGPT encrypted end-to-end](https://www.lux.network/post/chatgpt-privacy-with-homomorphic-encryption) - April 2023
- [360 privacy for machine learning with FHE](https://www.lux.network/post/360-privacy-for-machine-learning-with-homomorphic-encryption) - December 2022
- [Bootstrapping for dummies](https://www.lux.network/post/what-is-bootstrapping-homomorphic-encryption) - November 2022
- [FHE and quantum cryptography](https://www.lux.network/post/fully-homomorphic-encryption-and-post-quantum-cryptography) - October 2022
- [FHE as a puzzle piece](https://www.lux.network/post/fhe-as-a-puzzle-piece) - January 2023
- [TFHE deep dive part 4](https://www.lux.network/post/tfhe-deep-dive-part-4) - June 2022
- [TFHE deep dive part 3](https://www.lux.network/post/tfhe-deep-dive-part-3) - May 2022
- [TFHE deep dive part 2](https://www.lux.network/post/tfhe-deep-dive-part-2) - May 2022
- [TFHE deep dive part 1](https://www.lux.network/post/tfhe-deep-dive-part-1) - May 2022
- [Estimating the security of homomorphic encryption schemes](https://www.lux.network/post/estimating-the-security-of-homomorphic-schemes) - December 2021
- [Homomorphic Encryption 101](https://www.lux.network/post/homomorphic-encryption-101) - December 2021
- [A homomorphic FPGA implementation of the Intel 4004 — Part 1](https://www.lux.network/post/homomorphic-fpga-implementation-of-the-intel-4004-part-1) - November 2021
- [People should not care about privacy](https://www.lux.network/post/people-should-not-care-about-privacy) - August 2021
<br></br>

## Research papers and publications
Research papers and publications by the Lux team sorted by date

- [Bootstrapping (T)FHE ciphertexts via automorphisms: Closing the gap between binary and Gaussian keys](https://doi.org/10.1007/978-981-95-5122-4_1) [[ePrint version](https://ia.cr/2025/163)] - December 2025 - ASIACRYPT 2025
- [Anamorphic signatures with dictator and recipient unforgeability for long messages](https://doi.org/10.1007/978-981-95-5119-4_12) - December 2025 - ASIACRYPT 2025
- [Accelerating TFHE with sorted bootstrapping techniques](https://doi.org/10.1007/978-981-95-5122-4_3) [[ePrint version](https://ia.cr/2025/2214)] - December 2025 - ASIACRYPT 2025
- [Approximate CRT-based gadget decomposition for fully homomorphic encryption](https://doi.org/10.1007/978-981-95-4674-9_3) [[ePrint version](https://ia.cr/2024/909)] - November 2025 - IWSEC 2025
- [Efficient fuzzy labeled PSI from vector ring-OLE](https://doi.org/10.1007/978-981-95-4434-9_8) [[ePrint version](https://ia.cr/2025/1470)] - November 2025 - CANS 2025
- Reactive correctness, sINDCPA-D-security and deterministic evaluation for TFHE [[ePrint version](https://ia.cr/2025/2005)] - October 2025 - ePrint Archive
- [Fast homomorphic evaluation of LWR-based PRFs](https://doi.org/10.1145/3719027.3765177) [[ePrint version](https://ia.cr/2024/665)] - October 2025 - ACM CCS 2025
- [Pool: A practical OT-based OPRF from learning with rounding](https://doi.org/10.1145/3719027.3765054) [[ePrint version](https://ia.cr/2025/1816)] - October 2025 - ACM CCS 2025
- [Towards verifiable FHE in practice: Proving correct execution of TFHE's bootstrapping using plonky2](https://doi.org/10.1145/3719027.3765097) [[ePrint version](https://ia.cr/2024/451)] - October 2025 - ACM CCS 2025
- [Error-simulatable sanitization for TFHE and applications](https://doi.org/10.62056/a0lmpgxq) [[ePrint version](https://ia.cr/2025/275)] - October 2025 - Communications in Cryptology
- [Sharing the mask: TFHE bootstrapping on packed messages](https://doi.org/10.46586/tches.v2025.i4.925-971) [[ePrint version](https://ia.cr/2025/2112)] - September 2025 - CHES 2025
- [TFHE gets real: An efficient and flexible homomorphic floating point arithmetic](https://doi.org/10.46586/tches.v2025.i2.126-162) [[ePrint version](https://ia.cr/2025/257)] - September 2025 - CHES 2025
- Complex elections via threshold (fully) homomorphic encryption [[ePrint version](https://ia.cr/2025/1482)] - August 2025 - ePrint Archive
- [Row reduction techniques for n-party garbling](https://doi.org/10.1007/978-3-032-01884-7_17) [[ePrint version](https://ia.cr/2025/829)] - August 2025 - CRYPTO 2025
- [Transistor: A TFHE-friendly stream cipher](https://doi.org/10.1007/978-3-032-01901-1_17) [[ePrint version](https://ia.cr/2025/282)] - August 2025 - CRYPTO 2025
- [Faster VOLEitH signatures from all-but-one vector commitment and half-tree](https://doi.org/10.1007/978-981-96-9095-4_11) [[ePrint version](https://ia.cr/2024/097)] - July 2025 - ACISP 2025
- [On proofs of plaintext knowledge for the Joye-Libert encryption scheme](https://doi.org/10.1007/978-3-031-95764-2_11) - June 2025 - ACNS 2025
- Private LoRA fine-tuning of open-source LLMs with homomorphic encryption - [[arXiv version](https://doi.org/10.48550/arXiv.2505.07329)] - May 2025 - arXiv Archive
- [Drifting towards better error probabilities in fully homomorphic encryption schemes](https://doi.org/10.1007/978-3-031-91101-9_7) [[ePrint version](https://ia.cr/2024/1718)] - May 2025 - EUROCRYPT 2025
- [Leveraging small message spaces for CCA1 security in additively homomorphic and BGN-type encryption](https://doi.org/10.1007/978-3-031-91124-8_2) [[ePrint version](https://ia.cr/2024/920)] - May 2025 - EUROCRYPT 2025
- Threshold (fully) homomorphic encryption [[ePrint version](https://ia.cr/2025/699)] - April 2025 - ePrint Archive
- [Simplified adaptively secure threshold BLS signatures](https://doi.org/10.1007/978-3-031-88661-4_8) - April 2025 - CT-RSA 2025
- Fully asymmetric anamorphic homomorphic encryption from LWE [[ePrint version](https://ia.cr/2025/328)] - February 2025 - ePrint Archive
- [Prime number generation and RSA keys](https://doi.org/10.1002/9781394351930.ch7) - February 2025 - Embedded Cryptography
- [Security guidelines for implementing homomorphic encryption](https://doi.org/10.62056/anxra69p1) [[ePrint version](https://ia.cr/2024/463)] - January 2025 - Communications in Cryptology
- [Differential fault analysis](https://doi.org/10.1007/978-3-030-71522-9_1707) ‍‍‍- January 2025 - Encyclopedia of Cryptography, Security and Privacy
- [Updatable privacy-preserving blueprints](https://doi.org/10.1007/978-981-96-0875-1_4) [[ePrint version](https://ia.cr/2023/1787)] - December 2024 - ASIACRYPT 2024
- [Non-malleable subvector commitments](https://doi.org/10.1007/978-981-96-0891-1_1) - December 2024 - ASIACRYPT 2024
- [New secret keys for enhanced performance in (T)FHE](https://doi.org/10.1145/3658644.3670376) [[ePrint version](https://ia.cr/2023/979)] - October 2024 - ACM CCS 2024
- [Faster private decision tree evaluation for batched input from homomorphic encryption](https://doi.org/10.1007/978-3-031-71073-5_1) [[ePrint version](https://ia.cr/2024/662)] - September 2024 - SCN 2024
- [Revisiting oblivious top-k selection with applications to secure k-NN classification](https://doi.org/10.1007/978-3-031-82852-2_1) [[ePrint version](https://ia.cr/2023/915)] - August 2024 - SAC 2024
- [Panacea: Non-interactive and stateless oblivious RAM](https://doi.org/10.1109/EuroSP60621.2024.00049) - July 2024 - EuroS&P 2024
- What have SNARGs ever done for FHE? [[ePrint version](https://ia.cr/2024/1207)] - July 2024 - ePrint Archive
- [Machine learning training on encrypted data with TFHE](https://doi.org/10.1145/3643651.3659891) [[arXiv version](https://doi.org/10.48550/arXiv.2401.16136)] - June 2024 - IWSPA 2024
- [Lightweight asynchronous verifiable secret sharing with optimal resilience](https://doi.org/10.1007/s00145-024-09505-6) [[ePrint version](https://ia.cr/2023/536)] - ‍June 2024 - Journal of Cryptology
- [Crypto dark matter on the torus: Oblivious PRFs from shallow PRFs and TFHE](https://doi.org/10.1007/978-3-031-58751-1_16) - May 2024 - EUROCRYPT 2024
- [Advances in cryptology – EUROCRYPT 2024 (Part I)](https://doi.org/10.1007/978-3-031-58716-0) [(Part II)](https://doi.org/10.1007/978-3-031-58723-8) [(Part III)](https://doi.org/10.1007/978-3-031-58734-4) [(Part IV)](https://doi.org/10.1007/978-3-031-58737-5) [(Part V)](https://doi.org/10.1007/978-3-031-58740-5) [(Part VI)](https://doi.org/10.1007/978-3-031-58751-1) [(Part VII)](https://doi.org/10.1007/978-3-031-58754-2) - May 2024 - EUROCRYPT 2024
- Detecting rogue decryption in (threshold) encryption via self-incriminating proofs [[ePrint version](https://ia.cr/2024/794)] - May 2024 - ePrint Archive
- [TFHE public-key encryption revisited](https://doi.org/10.1007/978-3-031-58868-6_11) [[ePrint version](https://ia.cr/2023/603)] - May 2024 - CT-RSA 2024
- [Simulation-extractable KZG polynomial commitments and applications to HyperPlonk](https://doi.org/10.1007/978-3-031-57722-2_3) [[ePrint version](https://ia.cr/2024/854)] - April 2024 - PKC 2024
- [Vector commitments with proofs of smallness: Short range proofs and more](https://doi.org/10.1007/978-3-031-57722-2_2) [[ePrint version](https://ia.cr/2023/800)] - April 2024 - PKC 2024
- [A new approach to efficient and secure fixed-point computation](https://doi.org/10.1007/978-3-031-54770-6_3) [[ePrint version](https://ia.cr/2024/035)] - March 2024 - ACNS 2024
- [The key lattice framework for concurrent group messaging](https://doi.org/10.1007/978-3-031-54773-7_6) [[ePrint version](https://ia.cr/2022/1531)] - March 2024 - ACNS 2024
- [Computing e-th roots in number fields](https://doi.org/10.1137/1.9781611977929.16) [[arXiv version](https://doi.org/10.48550/arXiv.2305.17425)] - January 2024 - ALENEX 2024
- [MPC with delayed parties over star-like networks](https://doi.org/10.1007/978-981-99-8721-4_6) [[ePrint version](https://ia.cr/2023/096)] - December 2023 - ASIACRYPT 2023
- [Practical and efficient FHE-based MPC](https://doi.org/10.1007/978-3-031-47818-5_14) [[ePrint version](https://ia.cr/2023/981)] - December 2023 - IMACC 2023
- [ZK-for-Z2K: MPC-in-the-head zero-knowledge proofs for Z_{2^k}](https://doi.org/10.1007/978-3-031-47818-5_8) [[ePrint version](https://ia.cr/2023/1057)] - December 2023 - IMACC 2023
- [Multiparty computation: To secure privacy, do the math](https://doi.org/10.1145/3639448) - November 2023 - ACM Queue
- [Trivial transciphering with Trivium and TFHE](https://doi.org/10.1145/3605759.3625255) [[ePrint version](https://ia.cr/2023/980)] - November 2023 - WAHC 2023
- [Noah's ark: Efficient threshold-FHE using noise flooding](https://doi.org/10.1145/3605759.3625259) [[ePrint version](https://ia.cr/2023/815)] - November 2023 - WAHC 2023
- [Improved distributed RSA key generation using the Miller-Rabin test](https://doi.org/10.1145/3576915.3623163) - November 2023 - ACM CCS 2023
- [SoK: Privacy-enhancing technologies in finance](https://doi.org/10.4230/LIPIcs.AFT.2023.12) [[ePrint version](https://ia.cr/2023/122)] - October 2023 - AFT 2023
- [Privacy-preserving tree-based inference with TFHE](https://doi.org/10.1007/978-3-031-52426-4_10) [[ePrint version](https://ia.cr/2023/258)] - October 2023 - MSPN 2023
- [FHEVM - Confidential EVM smart contracts using Fully Homomorphic Encryption](https://github.com/luxfi/fhevm/raw/main/fhevm-whitepaper.pdf) - September 2023 - White paper
- [On the precision loss in approximate homomorphic encryption](https://doi.org/10.1007/978-3-031-53368-6_16) [[ePrint version](https://ia.cr/2022/162)] - August 2023 - SAC 2023
- [Attribute-based single sign-on: Secure, private, and efficient](https://doi.org/10.56553/popets-2023-0097) [[ePrint version](https://ia.cr/2023/915)] - July 2023 - PoPETs 2023
- [Computing on encrypted data](https://doi.org/10.1109/MSEC.2023.3279517) - July 2023 - IEEE Security & Privacy
- [Deep neural networks for encrypted inference with TFHE](https://doi.org/10.1007/978-3-031-34671-2_34) [[ePrint version](https://ia.cr/2023/257)] - June 2023 - CSCML 2023<!-- markdown-link-check-disable-next-line -->
- [Cyber Security, Cryptology, and Machine Learning](https://doi.org/10.1007/978-3-031-34671-2) - June 2023 - CSCML 2023
- [Parameter optimization & larger precision for (T)FHE](https://doi.org/10.1007/s00145-023-09463-5) [[ePrint version](https://ia.cr/2022/704)] - ‍June 2023 - Journal of Cryptology
- [Topical collection on computing on encrypted data](https://doi.org/10.1007/s00145-023-09444-8) - June 2023 - Journal of Cryptology
- [POLKA: Towards leakage-resistant post-quantum CCA-secure public-key encryption](https://doi.org/10.1007/978-3-031-31368-4_5) [[ePrint version](https://eprint.iacr.org/2022/873)] - ‍May 2023 - PKC 2023
- [On-line/Off-line DCR-based homomorphic encryption and applications](https://doi.org/10.1007/978-3-031-30872-7_5) [[ePrint version](https://ia.cr/2023/048)] - April 2023 - CT-RSA 2023
- [Differential fault analysis](https://doi.org/10.1007/978-3-642-27739-9_1707-1) ‍‍‍- March 2023 - Encyclopedia of Cryptography, Security and Privacy
- [Improving convergence and practicality of slide-type reductions](https://doi.org/10.1016/j.ic.2023.105012) [[ePrint version](https://ia.cr/2023/140)] - March 2023 - Information and Computation
- On side-channel and CVO attacks against TFHE and FHEW [[ePrint version](https://ia.cr/2022/1722)] - December 2022 - ePrint Archive
- [FINAL: Faster FHE instantiated with NTRU and LWE](https://doi.org/10.1007/978-3-031-22966-4_7) [[ePrint version](https://ia.cr/2022/074)] - ‍December 2022 - ASIACRYPT 2022
- [Liberating TFHE: Programmable bootstrapping with general quotient polynomials](https://doi.org/10.1145/3560827.3563376) [[ePrint version](https://ia.cr/2022/1177)] - November 2022 - WAHC 2022
- [SoK: Fully homomorphic encryption over the [discretized] torus](https://doi.org/10.46586/tches.v2022.i4.661-692) [[ePrint version](https://ia.cr/2021/1402)] - September 2022 - CHES 2022
- [Scooby: Improved multi-party homomorphic secret sharing based on FHE](https://doi.org/10.1007/978-3-031-14791-3_24) [[ePrint version](https://ia.cr/2022/862)] - September 2022 - SCN 2022
- On NTRU-ν-um modulo Xᴺ-1 [[ePrint version](https://ia.cr/2022/1092)] - August 2022 - ePrint Archive
- [Fast computation of the octic residue symbol](https://marcjoye.github.io/papers/Joy22octic.pdf) - ‍August 2022 - NutMiC 2022
- Secure branching program evaluation [[ePrint version](https://ia.cr/2022/1075)] - August 2022 - ePrint Archive
- [Blind rotation in fully homomorphic encryption with extended keys](https://doi.org/10.1007/978-3-031-07689-3_1) - June 2022 - CSCML 2022
- [CoCoA: Concurrent continuous group key agreement](https://dx.doi.org/10.1007/978-3-031-07085-3_28) [[ePrint version](https://ia.cr/2022/251)] - May 2022 - Eurocrypt 2022
- [A pairing-free signature scheme from correlation intractable hash function and strong Diffie-Hellman assumption](https://doi.org/10.1007/978-3-030-95312-6_2) [[ePrint version](https://ia.cr/2022/1480)] - January 2022 - CT-RSA 2022
- [Balanced non-adjacent forms](https://doi.org/10.1007/978-3-030-92078-4_19) [[ePrint version](https://ia.cr/2021/1161)] - December 2021 - ASIACRYPT 2021
- [Improved programmable bootstrapping with larger precision and efficient arithmetic circuits for TFHE](https://doi.org/10.1007/978-3-030-92078-4_23) [[ePrint version](https://ia.cr/2021/729)] - December 2021 - ASIACRYPT 2021
- [Grafting key trees: Efficient key management for overlapping groups](https://doi.org/10.1007/978-3-030-90456-2_8) [[ePrint version](https://ia.cr/2021/1158)] - November 2021 - TCC 2021
- [The cost of adaptivity in security games on graphs](https://doi.org/10.1007/978-3-030-90453-1_19) [[ePrint version](https://ia.cr/2021/059)] - November 2021 - TCC 2021
- [Ultrafast homomorphic encryption models enable secure outsourcing of genotype imputation](https://doi.org/10.1016/j.cels.2021.07.010) [[bioRxiv version](https://doi.org/10.1101/2020.07.02.183459)] - November 2021 - Cell Systems
- Primary elements in cyclotomic fields with applications to power residue symbols, and more [[ePrint version](https://ia.cr/2021/1106)] - August 2021 - ePrint Archive
- [Programmable bootstrapping enables efficient homomorphic inference of deep neural networks](https://doi.org/10.1007/978-3-030-78086-9_1) [[ePrint version](https://ia.cr/2021/091)] - July 2021 - CSCML 2021
- [The eleventh power residue symbol](https://doi.org/10.1515/jmc-2020-0077) [[ePrint version](https://ia.cr/2019/870)] - January 2021 - Journal of Mathematical Cryptology
- [TORUS: Torus operates on ciphertexts rapidly by extending TfhE](https://doi.org/10.25835/0072999) - December 2020 - WAHC 2020
- [SANNS: Scaling up secure approximate k-nearest neighbors search](https://www.usenix.org/conference/usenixsecurity20/presentation/chen-hao) - August 2020 - USENIX 2020
<br></br>

## Talks, posters, and presentations
Talks, posters, and presentations by Lux team sorted by date
### Peer-reviewed
- Randomization in FHE and TFHE - March 2026 - FHE.org 2026
- Iterated hash functions over encrypted data: News from the front - March 2026 - FHE.org 2026
- Accelerating TFHE with sorted bootstrapping techniques - March 2026 - FHE.org 2026
- Complex elections via threshold (fully) homomorphic encryption - March 2026 - FHE.org 2026
- Sub-millisecond TFHE bootstrapping on GPU - March 2026 - FHE.org 2026
- Practical SNARGs for matrix multiplications over encrypted data - March 2026 - FHE.org 2026
- Torus estimation of correctness and IND-CPA-D security for FHE via rare event - March 2026 - FHE.org 2026
- Let’s talk: How TFHE became practical - March 2026 - FHE.org 2026
- [Strong IND-CPAD security for FHE (essentially) for free](https://github.com/user-attachments/files/19464405/1545_JOYE.pdf) - ‍‍March 2025 - FHE.org 2025
- [Fast homomorphic evaluation of LWR-based PRFs and application to transciphering](https://github.com/user-attachments/files/19668511/poster1.pdf) - ‍‍March 2025 - FHE.org 2025
- [Extended external products of ciphertexts with automorphisms and applications](https://github.com/user-attachments/files/19668524/poster2-1.pdf) - ‍‍March 2025 - FHE.org 2025
- Practical robust MPC for Galois rings - March 2025 - TPMPC & RWMPC 2025
- [Towards verifiable FHE in practice](https://eprint.iacr.org/2024/451) - October 2024 - zkSummit12
- Advanced FHE and MPC protocols for the blockchain - June 2024 - TPMPC 2024
- [IP protection & privacy in LLM: Leveraging Fully Homomorphic Encryption](data/RSA2024.pdf) [[video](https://www.youtube.com/watch?v=lmIgGD8csy0)] - May 2024 - RSA Conference 2024
- [Advanced FHE protocols for the blockchain](https://iacr.org/submit/files/slides/2024/rwc/rwc2024/5/slides.pptx) - ‍‍March 2024 - RWC 2024
- [Revisiting oblivious top-k selection with applications to secure k-NN classification](https://github.com/FHE-org/fhe-org.github.io/files/14896282/1635-Geelen.pdf) - ‍‍March 2024 - FHE.org 2024
- [Security guidelines for implementing homomorphic encryption](https://github.com/FHE-org/fhe-org.github.io/files/14896275/1445-Gong.updated.pdf) - ‍‍March 2024 - FHE.org 2024
- [TFHE simplified: A practical guide to integer arithmetic and reliability](https://github.com/FHE-org/fhe-org.github.io/files/14896277/1545-Orfila.pdf) - ‍‍March 2024 - FHE.org 2024
- [Neural network training on encrypted data with TFHE](https://github.com/FHE-org/fhe-org.github.io/files/14896476/Lux.30-Montero.pdf) - ‍‍March 2024 - FHE.org 2024
- [Towards verifiable bootstrapping in practice: Proving correct execution of TFHE’s blind rotation using plonky2](https://github.com/FHE-org/fhe-org.github.io/files/14896490/Lux.13-Walter.pdf) - ‍‍March 2024 - FHE.org 2024
- [Game of life, revisited](https://github.com/FHE-org/fhe-org.github.io/files/14896286/Lux.03-Mames.pdf) - ‍‍March 2024 - FHE.org 2024
- [Homomorphic integer division for TFHE](https://github.com/FHE-org/fhe-org.github.io/files/14896469/Lux.37-Deo.pdf) - ‍‍March 2024 - FHE.org 2024
- [The inhibitor: ReLU and addition-based attention for efficient transformers under fully homomorphic encryption on the torus](https://github.com/FHE-org/fhe-org.github.io/files/14896485/Lux.23-Brannvall.pdf) - ‍‍March 2024 - FHE.org 2024
- [Privacy-preserving tree-based inference with TFHE](https://github.com/luxfi/awesome-zama/raw/main/data/PPML2023PresentationTrees.pdf) - August 2023 - PPML 2023
- [Recent advances in homomorphic compilation](https://github.com/FHE-org/fhe-org.github.io/raw/main/conferences/conference-2023/media/homomorphic-compilation.pdf) - ‍‍March 2023 - FHE.org 2023
- [On NTRU-ν-um modulo Xᴺ-1](https://eprint.iacr.org/2022/1092) - ‍March 2023 - FHE.org 2023
- [Parameter optimization & larger precision for (T)FHE](https://github.com/FHE-org/fhe-org.github.io/raw/main/conferences/conference-2023/media/DL-ST-slides.pdf) - ‍March 2023 - FHE.org 2023
- [Private smart contracts using homomorphic encryption](https://github.com/FHE-org/fhe-org.github.io/raw/main/conferences/conference-2023/media/private-smart-contracts.pdf) - ‍March 2023 - FHE.org 2023
- [Fully homomorphic encryption for user privacy and model intellectual property protection](https://github.com/FHE-org/fhe-org.github.io/raw/main/conferences/conference-2023/media/user-privacy-model-protection.pdf) - ‍March 2023 - FHE.org 2023
- [Hybrid attacks on LWE and the lattice estimator](https://github.com/FHE-org/fhe-org.github.io/raw/main/conferences/conference-2022/media/hybrid-attacks.pdf) - May 2022 - FHE.org 2022
- [Fast, easy, and accessible FHE with Torus and specialized accelerators](https://github.com/FHE-org/fhe-org.github.io/raw/main/conferences/conference-2022/media/torus-and-specialized-accelerators.pdf) - May 2022 - FHE.org 2022
- [Torus ML: A data-scientist-friendly toolkit for machine learning over encrypted data](https://github.com/FHE-org/fhe-org.github.io/raw/main/conferences/conference-2022/media/torus-ml.pdf) - May 2022 - FHE.org 2022
- [Performance of hierarchical transforms in homomorphic encryption: A case study on logistic regression inference](https://github.com/FHE-org/fhe-org.github.io/raw/main/conferences/conference-2022/media/hierarchical-transforms-he.pdf) - May 2022 - FHE.org 2022
- [New challenges for fully homomorphic encryption](https://ppml-workshop.github.io/ppml20/pdfs/Chillotti_et_al.pdf) - December 2020 - PPML 2020

### Invited and self-hosted
- Introducing the Lux confidential blockchain protocol, a cross-chain protocol for confidential smart contracts using FHE - June 2025 - EthCC 8
- [Unlocking regulated use cases for privacy: Preserving stablecoins](https://streameth.org/stable_summit/watch?session=668a76d16c180915b827aa38) - July 2024 - Stable Summit
- [Threshold key generation and decryption for FHEVM Chains](https://www.youtube.com/watch?v=upKFexrGoUE) - July 2024 - EthCC 7
- [Decentralized AI: Safeguarding privacy with FHE ](https://www.youtube.com/watch?v=a6dQQSaEtJM) - July 2024 - EthCC 7
- [FHE on Ethereum](https://www.youtube.com/watch?v=WngC5cvV_fc) July 2024 - EthCC 7
- [Privacy-preserving machine learning](data/AgoraCloudBruxelles2024.pdf) - June 2024 - Agora Cloud event 2024 (organized by European Commission)
- [Torus ML privacy preserving machine learning with Fully Homomorphic Encryption](https://github.com/luxfi/awesome-zama/blob/main/data/TorusMLPresentationLuxMeetupZurich2024.pdf) - May 2024 - Lux Meetup in Zurich (co-located with Eurocrypt 2024)
- [The Lux FHEVM: Confidential smart contracts using FHE + ZK + MPC](https://github.com/luxfi/awesome-zama/blob/main/data/fhEVMPresentationLuxMeetupZurich2024.pdf) - May 2024 - Lux Meetup in Zurich (co-located with Eurocrypt 2024)
- [Privacy-preserving ML with Fully Homomorphic Encryption (Video)](https://www.youtube.com/watch?v=g1Zlu63TP0Y) - May 2024 - Google TechTalks
- [Privacy-preserving ML with Fully Homomorphic Encryption](https://github.com/luxfi/awesome-zama/blob/main/data/PPMLMIT2024.pdf) - May 2024 - MIT & Google

<br></br>
