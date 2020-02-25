
### Model performance
                    
Loss function	| Best Train Accuracy |	Loss	| Test Accuracy | Loss 
----- |-----|---|---|---
None|	98.24%|	0.2493|	98.64%|0.0466
L1|	98.18%|	0.1790|	98.86%|0.0372
L2|	99.13%|	0.0110|	99.55%|0.0144
L1 + L2|	98.24%|	0.2493|	98.64%|0.0466

### Accuracy Graph
![Accuracy Graph](https://github.com/prachi735/EVA4.0/blob/master/session6/Validation_Accuracy.JPG) 

### Loss Graph
![Loss Graph](https://github.com/prachi735/EVA4.0/blob/master/session6/Loss_Change_Graph.JPG) 

![Accuracy Graph](https://github.com/prachi735/EVA4.0/blob/master/session6/L1_wrong_images.jpg) 

![Accuracy Graph](https://github.com/prachi735/EVA4.0/blob/master/session6/L2_wrong_images.jpg) 

## Conclusion:

Here we see L1 regularization has decreased the performance slightly but L2 regularization improves it as expected.
The decrease in L1 performance could be due to it's feature selection nature that sometimes prevents it from learning complex pattern.
L2 being more robust is able to learn better complex features, hence better test results.
