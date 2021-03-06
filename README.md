# pyGibbsLDA
Python Implementation of Collapsed Gibbs Sampling for Latent Dirichlet Allocation (LDA)

## Develop environment
* Language: Python3
* Prerequisite libraries: [Scipy](http://scipy.org), [Numpy](http://numpy.org), [matplotlib](http://matplotlib.org)

## Input data format
DocumentID \t WordID \t Count \n

## Module usage example
```python
>>> import GibbsLDA
>>> sampler = GibbsLDA.Sampler("/home2/TwitterData.dat", 100)
>>> likelihood = sampler.run(500, 300, 2)
```
* 100: # of topics
* 500: # of Gibbs samples
* 300: burn-in point
* 2: sampling interval

## Reference
* [http://www.cs.columbia.edu/~blei/papers/BleiNgJordan2003.pdf](http://www.cs.columbia.edu/~blei/papers/BleiNgJordan2003.pdf)
* [http://parkcu.com/blog/gibbs-sampling-for-topic-models](http://parkcu.com/blog/gibbs-sampling-for-topic-models)