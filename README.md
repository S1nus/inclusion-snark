# Inclusion Snark
1. Circuit takes all the shares of a blob as private inputs, and a Celestia data root as ***the only*** public input.
2. The proof data will be hashed along with the proof data from an arbitrary ZK rollup
3. The hash will be used to calculate a challenge point
4. The ZK rollup's outermost verifier (or proof aggregator) will verify the two proofs, and open challenge points from each instance, corresponding to the index of the private input from the rollup's pubdata, deterined by the hash.
5. [Equivalence is proved](https://ethresear.ch/t/easy-proof-of-equivalence-between-multiple-polynomial-commitment-schemes-to-the-same-data/8188?u=colludingnode)
