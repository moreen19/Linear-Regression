# Linear-Regression
A real life business case scenario solved through linear regression(full project file attached in files section)

Business case study

A business sells cloths online.Customers walk in the store, have meetings with the personal stylist and then they go home and order online either on the mobile app or the website
Business problem statement

The business is trying to decide on whether to develope the mobile app or the website since it does not have the funds to do both.

Machine learning solution

The following project is an ML based prediction analysis for the company to use to build a model to determine whether they should focus on the mobile app or website.This analysis may also provide other business insights that can help improve customer understanding and lead to appropriate business actions

**Time spent on app appears to have some correlation to yearly amount spent while time on website doesn't**

![image](https://github.com/moreen19/Linear-Regression/assets/97608840/66250dc3-b424-4925-adba-453d6aaa5aa0)

**Training the data**

from sklearn.linear_model import LinearRegression

create an instance of the LinearRegression n.b - we are using the linear regression algorithm to train our data

lm=LinearRegression()

**train or fit the data**

lm.fit(x_train,y_train)

**Predicting Test data**

predictions=lm.predict(x_test)

![image](https://github.com/moreen19/Linear-Regression/assets/97608840/881e841c-c698-466d-8b67-5ddf42f1e986)

## Conclusion

the coefficients will give us the answer on whether the company need to focus on the mobile app or the website

coefficients=pd.DataFrame(lm.coef_,x.columns)

coefficients.columns = ['coefficients']

coefficients

Length of Membership	61.279097

Time on App	38.590159

Time on Website	0.190405

Avg. Session Length	25.981550

We should develop the App though the coefficients show that length of membership has the most effect on the yearly amount spent at the store by customers

