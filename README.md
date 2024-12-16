# Isogenies computation over twist curves for BLS24 and BLS48 curves

This repository presents a novel technique for finding isogenous curves over high-order extension fields, specifically for pairing-friendly curves. The proposed approach constructs isomorphic fields and curves corresponding to the target ones, computes isogenies on the new curves, and maps the results back to the original extension field. The discovered isogenies are further utilized to implement simplified SWU mapping techniques for points on torsion subgroups defined by twist curves in BLS24 and BLS48. The results, extensively benchmarked and highly promising, are documented in .ipynb files designed for execution in a SageMath kernel. These findings have also been detailed in the newly submitted paper, **"Extending Constant-Time Simplified SWU Mapping to handle Twists of BLS24 and BLS48 Pairing-Friendly Curves"**.

### Representation of Extension Field Elements

**Note:** Elements of the extension fields Fp4 and Fp8 are represented as vectors of elements from the corresponding Fp field:

- **For Fp4:**  
  An element x is represented as:  
  `x = [a0, a1, a2, a3]`  
  corresponding to: `(a0 + a1*u) + (a2 + a3*u)*v`

- **For Fp8:**  
  An element x is represented as:  
  `x = [a0, a1, a2, a3, a4, a5, a6, a7]`  
  corresponding to: `(a0 + a1*u) + (a2 + a3*u)*v + ((a4 + a5*u) + (a6 + a7*u)*v)*w`


---

Proposed and implemented by  FARAOUN Kamel Mohamed
kamel_mh@yahoo.fr  
EEDIS Laboratory
UDL-University
