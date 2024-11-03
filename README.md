Supplementary Material to: Quantum CORDIC - Arcsin on a Budget
===

### Iain Burge, Institut Polytechnique de Paris, France.

### Michel Barbeau, Carleton University, School of Computer Science, Canada.

### Joaquin Garcia-Alfaro, Institut Polytechnique de Paris, France.

## Abstract

This work introduces a quantum algorithm for computing the arcsine
function to an arbitrary accuracy. We leverage
a technique from embedded computing and field-programmable
gate array (FPGA), called COordinate Rotation DIgital Computer
([CORDIC](https://en.wikipedia.org/wiki/CORDIC)). CORDIC is a family of iterative algorithms
that, in a classical context, can approximate various trigonometric,
hyperbolic, and linear functions using only bit shifts and
additions. Adapting CORDIC to the quantum context is non-trivial,
as the algorithm traditionally uses several non-reversible
operations. We detail a method for CORDIC which avoids such
non-reversible operations. We propose multiple approaches to
calculate the arcsine function reversibly with CORDIC. For $n$ bits
of precision, our method has space complexity of order n qubits,
a layer count in the order of n times log n, and a CNOT count in
the order of n squared. This primitive function is a required step
for the [Harrow–Hassidim–Lloyd](https://en.wikipedia.org/wiki/HHL_algorithm) (HHL) algorithm, is necessary
for quantum digital-to-analog conversion, can simplify a quantum
speed-up for Monte-Carlo methods, and has direct applications
in the quantum estimation of Shapley values.

*Keywords:* Quantum Algorithm, Quantum Computing, Quantum Information.

*Version:* October 30, 2024

### Updated code

All the code related to this work is available in <a href="https://github.com/iain-burge/QuantumCORDIC/tree/main/code">this repository</a>.

### Experimental results

We conducted some python simulations and found that the maximum error
for any given input can be made arbitrarily small by making $n$ larger
(see Figure 1). The full codebase can be found in this [GitHub repository](https://github.com/iain-burge/QuantumCORDIC/tree/main/code),
releasing a complete implementation of our proposal using Qiskit, as
well as an identical classical implementation.

![](img/results.png?raw=true)

#### Figure 1. Results of both Quantum and Classical simulations of Quantum compatible Algorithm for CORDIC Arcsine (cf. python code [here](https://github.com/iain-burge/QuantumCORDIC/tree/main/code)). (a) Quantum simulation, $n=4$. (b) Quantum simulation, $n=5$. (c) Quantum simulation, $n=6$. (d) Classical simulation, $n=6$. (e) Classical simulation, $n=10$. (f) Classical simulation, $n=16$.


## References

If using this code for research purposes, please cite:

[1] I. Burge, M. Barbeau, J. Garcia-Alfaro. "Quantum CORDIC - Arcsin on a Budget". *To Appear in 2025*.


```
@InProceedings{burge2024cordic,
  title={Quantum CORDIC --- Arcsin on a Budget},
  author={Burge, Iain and Barbeau, Michel and Garcia-Alfaro, Joaquin},
  booktitle={},
  year={2025},
  month={},
  publisher={IEEE},
  doi = {},
  url = {},
}
```


