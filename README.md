# CSS 314 – Parallel Computing & Performance Optimization

This project evaluates memory hierarchy, cache locality, false sharing, parallel scaling, and Roofline performance using Python and multiprocessing.

The experiments compare memory access patterns, loop interchange, padded and unpadded shared memory counters, strong and weak scaling, and arithmetic intensity. The results demonstrate the performance impact of memory access patterns and parallel execution overhead on Apple Silicon hardware.

All experimental measurements and numerical verification outputs are stored in the `results/` directory.

(.venv) alinaamangeldieva@MacBook-Pro-Alina CS482_Lab % python3 verify_outputs.py
============================================================
CS482 Parallel Computing: Automated Practicum Verifier
============================================================
[PASS] Milestone 0 (Host & Salt): Topology verified. Student ID: 230103224 | Salted N: 1472
[PASS] Milestone 1 (Locality & Interchange): Stride cliff reproduced: Stride-8 is 1.00x slower per element than Stride-1
[PASS] Milestone 1 (Locality & Interchange): Loop interchange speedup verified: 5.17x (Naive: 0.28s -> i-k-j: 0.05s)
[PASS] Milestone 2 (False Sharing & Karp-Flatt): Telemetry loaded, raw columns verified.
[PASS] Milestone 3 (Scaling & Roofline): Roofline analysis complete. AI: 0.10416666666666667 FLOPs/byte | Regime: memory-bound

============================================================
[COMPLETE] All milestones verified successfully!
Generated submission receipt: results/verification_receipt.sig
Token: 589fef86a14194dd...
============================================================
