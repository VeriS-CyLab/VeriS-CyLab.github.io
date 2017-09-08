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


## Kelinci

- **Upcoming paper:** Rody Kersten, Kasper Luckow, Corina Pasareanu. **AFL-based Fuzzing for Java with Kelinci**. To be presented as a poster at [https://www.sigsac.org/ccs/CCS2017](CCS 2017).
- **Link:** [https://github.com/isstac/kelinci](https://github.com/isstac/kelinci)

Grey-box fuzzing is a random testing technique that has been shown to be effective at finding security vulnerabilities in software. The technique leverages program instrumentation to gather information about the program with the goal of increasing the code coverage during fuzzing, which makes gray-box fuzzers extremely efficient vulnerability detection tools. One such tool is AFL, a grey-box fuzzer for C programs that has been used successfully to find security vul- nerabilities and other critical defects in countless software products.  We present Kelinci, a tool that interfaces AFL with instrumented Java programs. The tool does not require modifications to AFL and is easily parallelizable. Applying AFL-type fuzzing to Java programs opens up the possibility of testing Java based applications using this powerful technique. We show the effectiveness of Kelinci by applying it on the image processing library Apache Commons Imaging, in which it identified a bug within one hour.
