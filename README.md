# lab4
1. Step-Decay
  if epoch == 40 | epoch == 60 | epoch == 80:
     return lr * 0.5
   else:
     return lr
     
     
validation - синий

train - оранжевый

![Image alt](https://github.com/ilyashka170100/lab4/blob/master/img/laba4_1_1.png)
![Image alt](https://github.com/ilyashka170100/lab4/blob/master/img/laba4_1_2.png)

2. Exponential Decay

 if epoch < 10:
   return lr
  else:
   return lr * tf.math.exp(-0.1)
   
validation - синий

train - оранжевый

![Image alt](https://github.com/ilyashka170100/lab4/blob/master/img/laba4_2_1.png)
![Image alt](https://github.com/ilyashka170100/lab4/blob/master/img/laba4_2_2.png)


3 Warm-Up
 initial_lrate = 0.00001
  drop = 0.5
  epochs_drop = 5.0
  start_lr = 0
  finish_lr = 0.000001
  if epoch <= 7:
    return epoch * (finish_lr - start_lr)/10
  else:
    return initial_lrate
   
validation - синий

train - оранжевый

![Image alt](https://github.com/ilyashka170100/lab4/blob/master/img/laba4_3_1.png)
![Image alt](https://github.com/ilyashka170100/lab4/blob/master/img/laba4_3_2.png)
  
 
    
    
   
