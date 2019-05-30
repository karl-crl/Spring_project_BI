# Spring_project_BI

## Project description

SPAN(Semi-supervised Peak ANalyzer) ---  is a tool for analyzing ChIP-seq / ATAC-seq data supporting ultra-low and single-cell input. SPAN creates 3 state HMM model to fit data. Zinba tool (http://genomebiology.com/2011/12/7/R67) use pretty simular model to fit data but it also provides an opportunity to add additional information about data such as GC-content, mappability, etc. In this project we want to approach this ability.
 
## Goals and objectives
The main aims of the project:
1) Study general linear models.
2) Create classes for model and add to bioinf_commons.
3) Implement model to SPAN.
4) Compare upgraded model to current version.
It's really big aims. During this semester I was able to complete first two aims.

## Completed tasks
1) Studied general linear models
2) Created class for weighted regression
3) Made pull request to Apache.Commons.Statistics with some additional features for weighted regression
4) Created abstract class for regression
5) Created class for poisson regression
6) Created class for mixture with three states: zero-inflated and two poissons.

## Results
To test mixture model and poisson regression we generated data frame with 2*10^6 random variables from [0,1]. Then we sample observation and using data frame and observation fit new mixture. 
Poisson regression:
	- Accuracy: 10^{-3}.
	- Average working time: 7.5 sec.
	- Number of iterations: 19.

Mixture model:
	- Accuracy: 10^{-3}.  
	- Average working time: 24.7 sec.
	- Number of iterations: $9$.
\end{itemize}
