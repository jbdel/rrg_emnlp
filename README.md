## Improving the Factual Correctness of Radiology Report Generation with Semantic Graph-Based Rewards

## Rebuttal
Please find the updated manuscript in "updated_manuscript.pdf" <br/>
Please find the our best result on mimic in "eval_mimic.ipynb" with output: <br/>

```
{
    "ROUGEL": 0.25957182933436834,
    "radgraph_simple": 0.3707634326584056,
    "radgraph_partial": 0.3473400863906501,
    "radgraph_complete": 0.23481543928467108,
    "radentitymatchexact": 0.42533178285691237,
    "radentitynli": 0.4329851069563082,
    "chexbert-5_micro avg_f1-score": 0.6215361255219537,
    "chexbert-all_micro avg_f1-score": 0.5600310338139264
}

```

### First submission
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
