---
layout: page
title: Software
use-site-title: true
---
This is an overview of the software produced by the Verified Software group. Please check out our organization on GitHub: [https://github.com/isstac](https://github.com/isstac).


## SPF-WCA

- **Paper:** Kasper Luckow, Rody Kersten, Corina Pasareanu. **Symbolic Complexity Analysis Using Context-Preserving Histories**. In *2017 IEEE International Conference on Software Testing, Verification and Validation (ICST)*. \[[DOI](https://doi.org/10.1109/ICST.2017.13)\]\[[BibTeX]({{ site.baseurl }}{% link publications/icst2017.bib %})\]\[[PDF]({{ site.baseurl }}{% link publications/icst2017.pdf %})\]. Received **Best Paper Award** 
- **Link:** [https://github.com/isstac/spf-wca](https://github.com/isstac/spf-wca)

SPF-WCA is a tool for scalable complexity analysis of programs. It relies on a combination of symbolic execution and regression analysis to estimate complexity bounds. Symbolic execution is used for finding the longest paths for increasing input sizes. The data set is then used with regression analysis to find the model that best fits the data. Scalability is achieved by using symbolic execution in two phases: In the first phase, exhaustive symbolic execution is applied for *small* input sizes (e.g., length of a list to be sorted). From these, SPF-WCA derives a *guidance policy* that succinctly captures the pattern of the decisions made on the longest paths. The guidance policy is used in the next phase to *prune* choices that are deemed unlikely to exercise the worst-case path.


