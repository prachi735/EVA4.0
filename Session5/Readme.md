# CODE 1
## Target: basic model with setup	
1. get test train data
2. set transforms
3. set data loaders
4. setup a simple model without any fancy stuff
5. set training & test loop
## Result:
Parameters: 77,562	
Best Train Accuracy: 99.87%	
Best Test Accuracy: 99.87%	
## Analysis: 
1. the best train and test accuracy are similar 
2. the number of parameters is too high"

# CODE 2
## Target: reduce parameters
1. Changed the kernels and layers to reducce the number of parameters
## Result:
Parameters: 7,690
Best Train Accuracy: 98.62%
Best Test Accuracy: 98.86%
## Analysis:
1. Training accuracy & test accuracy has decreased due to lesser parameters 
2. Model has capability to improve by increasing training accuracy

# CODE 3 
## Target: batchnorm	
Added the batchnorm after every convulution
## Result:
Parameters: 7,840	
Best Train Accuracy: 99.51%
Best Test Accuracy: 99.61%
## Analysis:
1. model performs good after the 10th epoch
2. we can try making model more efficient by introducing GAP

# CODE 4
## Target: Regularization 
Added dropout as regularization to push model even further and increase both train & test accuracy
## Result:
Parameters: 7,840
Best Train Accuracy: 98.97%
Best Test Accuracy: 99.45%
## Analysis: 
The model has reduced slightly here,
similare result were observed by adding gap layer, hence removed from final model

# CODE 5
## Target: data augmentation	
Added data augmentation to make model more robust			
## Result:
Parameters: 7,840
Best Train Accuracy: 98.93%
Best Test Accuracy: 99.48%
## Analysis:
The model accuracy has not increased but that is expected as we have made it harder for the model to train.


### Final Model layer: Input, Output, Receptive Field
                    
Layer	| Nin |	k	| p | s |	Nout | jout |	RF
----- |-----|---|---|---|----- |----- |---
input|	28|	0|	0|	0|	|	1|	1|
c1|	28|	3|	0|	1|	26|	1|	3|
c2|	26|	3|	0|	1|	24|	1|	5|
c3|	24|	3|	0|	1|	22|	1|	7|
p1|	22|	2|	0|	2|	11|	2|	9|
c4|	11|	1|	0|	1|	11|	2|	9|
c5|	11|	3|	0|	1|	9|	2|	13|
c6|	9|	3|	0|	1|	7|	2|	17|
c7|	7|	3|	0|	1|	5|	2|	21|
c8|	5|	5|	0|	1|	1|	2|	29|

Group:
Chandan Kumar,
Abhinav Rana,
Harsha Vardhan,
Prachi Singh
