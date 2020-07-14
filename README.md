# QuadraticResidueEncryption
A simple implementation of Goldwasser-Micali encryption in java.

The Goldwasser–Micali (GM) cryptosystem is an asymmetric key encryption algorithm developed by Shafi Goldwasser and Silvio Micali in 1982. GM has the distinction of being the first probabilistic public-key encryption scheme which is provably secure under standard cryptographic assumptions. However, it is not an efficient cryptosystem, as ciphertexts may be several hundred times larger than the initial plaintext. To prove the security properties of the cryptosystem, Goldwasser and Micali proposed the widely used definition of semantic security.
Goldwasser–Micali consists of three algorithms: a probabilistic key generation algorithm which produces a public and a private key, a probabilistic encryption algorithm, and a deterministic decryption algorithm.

The scheme relies on deciding whether a given value x is a square mod N, given the factorization (p, q) of N. This can be accomplished using the following procedure:

Compute xp = x mod p, xq = x mod q.
If {\displaystyle x_{p}^{(p-1)/2}\equiv 1{\pmod {p}}}x_{p}^{{(p-1)/2}}\equiv 1{\pmod  {p}} and {\displaystyle x_{q}^{(q-1)/2}\equiv 1{\pmod {q}}}x_{q}^{{(q-1)/2}}\equiv 1{\pmod  {q}}, then x is a quadratic residue mod N.
