# Machine Remaining Useful Life Prediction via an Attention-Based Deep Learning Approach

Chen, Z., Wu, M., Zhao, R., Guretno, F., Yan, R., & Li, X. (2020). 
Machine remaining useful life prediction via an attention-based deep learning approach. 
IEEE Transactions on Industrial Electronics, 68(3), 2521-2531.

### Tested Environment
```
python              3.9.19 
numpy               1.26.4
pandas              2.2.1
keras               3.2.0 
tensorflow          2.16.1
scikit-learn        1.4.2 
scipy               1.13.0 
matplotlib          3.8.4 
```

### Tested Results with `code_FD001.py`
```
...

Epoch 31/32
4/4 ━━━━━━━━━━━━━━━━━━━━ 0s 3ms/step 
555/555 ━━━━━━━━━━━━━━━━━━━━ 2s 4ms/step  
Test RMSE: 13.773359373087182  Test score: 346.9256846812021
178/178 - 6s - 31ms/step - loss: 0.0128 - mse: 0.0128

Epoch 32/32
4/4 ━━━━━━━━━━━━━━━━━━━━ 0s 3ms/step 
555/555 ━━━━━━━━━━━━━━━━━━━━ 2s 3ms/step  
Test RMSE: 14.353312183496199  Test score: 370.0512514015058

178/178 - 4s - 25ms/step - loss: 0.0125 - mse: 0.0125
4/4 ━━━━━━━━━━━━━━━━━━━━ 0s 3ms/step 
lastScore: 370.0512514015058 lastRMSE 14.353312183496199
```

### Tested Results with `code_FD004.py`
```
...

Epoch 29/30
8/8 ━━━━━━━━━━━━━━━━━━━━ 0s 3ms/step 
1689/1689 ━━━━━━━━━━━━━━━━━━━━ 5s 3ms/step  
Test RMSE: 24.075631225525495  Test score: 4435.054921920252
541/541 - 13s - 23ms/step - loss: 0.0227 - mse: 0.0227

Epoch 30/30
8/8 ━━━━━━━━━━━━━━━━━━━━ 0s 3ms/step 
1689/1689 ━━━━━━━━━━━━━━━━━━━━ 5s 3ms/step  
Test RMSE: 23.729253363996584  Test score: 4600.772345344595
541/541 - 13s - 23ms/step - loss: 0.0226 - mse: 0.0226

8/8 ━━━━━━━━━━━━━━━━━━━━ 0s 5ms/step 
lastScore: 4600.772345344595 lastRMSE 23.729253363996584
```

Data: 
data can be downloaded from NASA web: https://c3.nasa.gov/dashlink/resources/139/

To replicate the results reported in the paper (python 2.7)

pip install -r requirement

python code_FD001.py

python code_FD004.py

Note that: attention_utils.py can be downloaded from https://github.com/philipperemy/keras-attention-mechanism
