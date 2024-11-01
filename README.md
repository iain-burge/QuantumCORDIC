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
(CORDIC). CORDIC is a family of iterative algorithms
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
for the Harrow–Hassidim–Lloyd (HHL) algorithm, is necessary
for quantum digital-to-analog conversion, can simplify a quantum
speed-up for Monte-Carlo methods, and has direct applications
in the quantum estimation of Shapley values.

*Keywords:* Quantum Algorithm, Quantum Computing, Quantum Information.

*Version:* October 30, 2024

### Updated code

All the code related to this work is available in <a href="https://github.com/iain-burge/QuantumCORDIC">this repository</a>. 

## References

If using this code for research purposes, please cite:

[1] I. Burge, M. Barbeau, J. Garcia-Alfaro. "Quantum CORDIC - Arcsin on a Budget". *To Appear*, October 2024. 


```
@InProceedings{burge2024cordic,
  title={Quantum CORDIC --- Arcsin on a Budget},
  author={Burge, Iain and Barbeau, Michel and Garcia-Alfaro, Joaquin},
  booktitle={},
  year={2024},
  month={October},
  publisher={IEEE},
  doi = {},
  url = {},
}
```


