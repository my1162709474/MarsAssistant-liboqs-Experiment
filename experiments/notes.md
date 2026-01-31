# liboqs Experiment Notes

## Overview
Exploring post-quantum cryptography with liboqs library.

## What is liboqs?
- Open-source C library for quantum-resistant cryptography
- Implements NIST PQC finalists
- Prototyping and experimentation tool

## Key Algorithms

### Key Encapsulation (KEM)
| Algorithm | NIST Level | Ciphertext Size |
|-----------|------------|----------------|
| Kyber512 | Level 1 | ~1 KB |
| Kyber768 | Level 3 | ~1.5 KB |
| Kyber1024 | Level 5 | ~2 KB |

### Digital Signatures
| Algorithm | NIST Level | Signature Size |
|-----------|------------|----------------|
| Dilithium2 | Level 2 | ~2 KB |
| Dilithium3 | Level 3 | ~3 KB |
| Falcon512 | Level 1 | ~0.7 KB |
| SPHINCS+ | Level 1 | ~7 KB |

## Experiment Results

### Experiment 1: Kyber KEM
- Successfully demonstrated key encapsulation
- Based on Module-LWE problem
- NIST PQC finalist

### Experiment 2: Dilithium Signatures  
- Successfully demonstrated digital signatures
- Based on Module-LWE + Module-SIS
- NIST PQC finalist

### Experiment 3: Algorithm Comparison
- Kyber: Best for key exchange (small, fast)
- Dilithium: Best for signatures (balanced)
- Falcon: Smallest signatures, very fast verification
- SPHINCS+: Stateless, largest signatures

## Recommendations

### For Key Exchange
Use **Kyber512** - NIST Level 1, good balance of size/speed

### For Digital Signatures
Use **Dilithium2** - NIST Level 2, or **Falcon512** for small signatures

### For Complete Solution
Consider **Kyber + Dilithium** hybrid scheme

## Next Steps
1. Add performance benchmarks
2. Test with different security levels
3. Explore hybrid cryptographic schemes
4. Integration with existing systems

## References
- [liboqs GitHub](https://github.com/open-quantum-safe/liboqs)
- [Open Quantum Safe](https://openquantumsafe.org/)
- [NIST PQC](https://csrc.nist.gov/projects/post-quantum-cryptography)

---
*Experiment notes by MarsAssistant - 2026-01-31*
