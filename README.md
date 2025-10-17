# Implementation of Univariate Linear Regression
## Aim:
To implement univariate Linear Regression to fit a straight line using least squares.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1.	Get the independent variable X and dependent variable Y.
2.	Calculate the mean of the X -values and the mean of the Y -values.
3.	Find the slope m of the line of best fit using the formula.
 ![eqn1](./eq1.jpg)
4.	Compute the y -intercept of the line by using the formula:
![eqn2](./eq2.jpg)  
5.	Use the slope m and the y -intercept to form the equation of the line.
6.	Obtain the straight line equation Y=mX+b and plot the scatterplot.
## Program
```
## REGISTER NUMBER : 212224240061
## COMPLETED BY : JAYAPRADAN M



import numpy as np
X= np.array(eval(input()))
Y= np.array(eval(input()))
X_mean=np.mean(X)
Y_mean=np.mean(Y)
num=0
denom=0
for i in range(len(X)):
  num+=(X[i]-X_mean)*(Y[i]-Y_mean)
  denom=(X[i]-X_mean)**2
  m=num/denom
  c=Y_mean-m*X_mean
  print(m,c)
  Y_pred=m*X+c
  print(Y_pred)

  import matplotlib.pyplot as plt
  plt.scatter(X,Y,color='RED')
  plt.plot(X,Y_pred,color='blue')
  plt.show()





```
## Output

<img width="703" height="550" alt="image" src="https://github.com/user-attachments/assets/ab646913-e133-4244-a2e5-2601fe7e0080" />
<img width="641" height="510" alt="image" src="https://github.com/user-attachments/assets/cb003733-2132-4176-83ee-49b29f901e02" />
<img width="863" height="595" alt="image" src="https://github.com/user-attachments/assets/074c3764-b75c-432b-914b-a8cf7a25371f" />
<img width="646" height="511" alt="image" src="https://github.com/user-attachments/assets/d4067b33-cd45-4fe2-88ef-d9aa1a5a08f9" />
<img width="615" height="512" alt="image" src="https://github.com/user-attachments/assets/d472b35a-efdb-44de-9f70-e64ab5468582" />

</br>
</br>
</br>
</br>

## Result
Thus the univariate Linear Regression was implemented to fit a straight line using least squares.
