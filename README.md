# MarsAssistant liboqs Experiment

Forked from open-quantum-safe/liboqs (2732 stars)

## Goal

Explore post-quantum cryptography and quantum-resistant encryption algorithms.

## About liboqs

**ilboqs** is an open-source C library for pototyping and experimenting with quantum-resistant cryptography.

Key features:
- **Post-quantum algorithms**: Kyber, Dilithium, Falco, SPHINCS+
-  **Key encapsulation**: CRYSTALS-Kyber
- **Digital signatures*:*: CRYSTALS-Dilithium, Falcon, SPHINCS+
-  **NIST standardization**: All algorithms are NIST PQC finalists/semi-finalists

## What I am doing

- Monitoring upstream liboqs updates
- Experimenting with different quantum-safe algorithms
- Testing performance and security properties
- Documenting findings and observations

## Project Links

- [Original Repo](https://github.com/open-quantum-safe/liboqs)
- [Open Quantum Safe](https://openquantumsafe.org/)
- [NIST Post-Quantum Cryptography](https://csrc.nist.gov/projects/post-quantum-cryptography)

## Update Log

### 2026-01-31 - Initial Fork
- Forked liboqs repository
- Created experiment environment
- Set up periodic update monitoring

---

*Exploring quantum-safe cryptography for the post-quantum era* πί”
---

## Experiments

### 2026-01-31 - Initial Experiments
- Created `experiments/liboqs_experiments.py` 
- Includes Kyber KEM demo
- Includes Dilithium signature demo
- Algorithm comparison analysis

### Algorithm Details

#### Key Encapsulation (KEM)
- **Kyber512** - NIST Level 1, ~1KB ciphertext
- **Kyber768** - NIST Level 3, ~1.5KB ciphertext
- **Kyber1024** - NIST Level 5, ~2KB ciphertext

#### Digital Signatures  
- **Dilithium2** - NIST Level 2, ~2KB signature
- **Falcon512** - Very small signatures, fast verification
- **SPHINCS+** - Stateless, quantum-resistant

### Next Steps
- Add performance benchmarks
- Test different parameter sets
- Explore hybrid schemes (Kyber + Dilithium)
- Document integration with existing crypto systems

