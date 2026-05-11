# SGD-Classifier
## AIM:
To write a program to predict the type of species of the Iris flower using the SGD Classifier.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
```
1.Start the program.
2.Read two input numbers from the user:
  *.First number → A
  *.Second number → B
3.Perform addition operation:
  *.Add A and B
  *.Store the sum in a variable called Result
4.Display the value of Result on the screen.
5.Stop the program.

```

## Program:
```python
/*
Program to implement the prediction of iris species using SGD Classifier.
Developed by:sanjutha D 
RegisterNumber:212225240136


from sklearn import datasets
from sklearn.linear_model import SGDClassifier
from sklearn.model_selection import train_test_split
from sklearn.metrics import accuracy_score

iris = datasets.load_iris()
X = iris.data
Y = iris.target

X_train, X_test, Y_train, Y_test = train_test_split(X, Y, test_size=0.2, random_state=0)

model = SGDClassifier(max_iter=1000, learning_rate='optimal')
model.fit(X_train, Y_train)

Y_pred = model.predict(X_test)

print("Accuracy:", accuracy_score(Y_test, Y_pred))

sample = [X[0]]
prediction = model.predict(sample)

print("Predicted Species:", iris.target_names[prediction][0])  
*/
```

## Output:

<img width="773" height="62" alt="image" src="https://github.com/user-attachments/assets/5f66779c-bd98-417a-bc71-d791ee5a4969" />


## Result:
Thus, the program to implement the prediction of the Iris species using SGD Classifier is written and verified using Python programming.
