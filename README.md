# Improving the Factual Correctness of Radiology Report Generation with Semantic Graph-Based Rewards

`RadGraph.ipynb` will evaluate the output of a system against the reference report using the RadGraph metric (RG_ER and RG_\hat{ER}). It also prints the sets \hat{V}_\hat{y} and \hat{V}_y (similarly to Appendix B) <br/>


To not violate the double blind review process, we do not release the training code for now. RadGraph can be easily integrated in any RRG framework given the code in RadGraph.ipynb


**erratum**: Appendix C 'study' : 
```
Reader 1: 48.5 ± 66.2 
Reader 2: 89.1 ± 46.1
```
to 
```
Reader 1: 0.485 ±0.662 
Reader 2: 0.891 ± 0.461
```
