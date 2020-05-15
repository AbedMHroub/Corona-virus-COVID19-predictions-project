# Welcome to Corona virus (COVID19) predictions project !

**Note:** There is an explanation of the project and the results below.

>*Today, the world is facing a widespread spread of the corona virus and an increase in the number of infections and deaths due to this disease, wishing safety and health for all.*

> Note: This project is a research study and we are working on
> developing it and increasing the number of features used in training,
> as we only used today's number in the training process

**Aim :** Predict using ML the number of infected people and the number of deaths of coronavirus.

----
**Run:**
 - You can make **clone for this repo** and then **run via Jupyter.**

	  **Another way is faster:**
	  1. Go to the project's [Colaboratory from here](https://colab.research.google.com/drive/1utQ4n9YSYF07NSvGzfC5Ub5G4gXp2xQ3?usp=sharing)
	  2. Make your own copy for run.(File --> Save a copy in drive )
	  3. Run cell

----
**Technologies:**
 -  [Python 3.8.0](https://www.python.org/downloads/release/python-380/)
 -  [Jupyter](https://jupyter.org/)
 -  [Colaboratory](https://colab.research.google.com/drive/1utQ4n9YSYF07NSvGzfC5Ub5G4gXp2xQ3?usp=sharing)

**DataSet :** We used data for the **United States** to train our model and we got data for **95 days** that includes the date of the day and the number of people with the disease and for the data of the dead we got data for **60 days** and also includes the date of the day and the number of deaths due to disease.

![2020](https://user-images.githubusercontent.com/36266329/81307391-4887cc80-9089-11ea-98f4-e60e45ef6ce7.jpg)

The reference [worldometers](https://www.worldometers.info/coronavirus/country/us/)



**We used 3 types of ML models :**
 - *Linear regression with log values*
 - *Support Vector Regression (SVR)*
 - *Artificial Neutral Network (MLPRegressor)*
 

### Work methodology :
 - The data was divided into two sections, for **training** and 
   **testing** .
 - We adopted the **K-Fold Cross-validation** methodology when selecting
   the best parameter for a single model.
   The following figure shows the work methodology:
    ![us_data](https://user-images.githubusercontent.com/36266329/81294029-f0e06580-9076-11ea-9e34-aaa611913a78.png)

## Infected
When looking for data for the **United States - Active Cases (Total)**, we obtained data for 95 days, starting **21/1/2020** , and the number of injured was **one** and we assumed on the first day. The data ended on **25/4/2020**, today is 95, and the number of injured is **788,233**.

We took data for **12 days** randomly for the final **test and evaluation stage**. After that we trained the different models, got a **final evaluation** and represented them with **score for each model**.

*The following figure represents the **curve for each model** in addition to the **score** obtained:*
> **Note:** The data were represented using two methods, the first is a
> **logarithmic representation** and the second is a **Linear representation
> (Exponential)**. The models were trained in both methods, and we chose
> the best among them for each model individually.
> - When looking at the Linear Regression curve, we used logarithmic representation of data when training it, and the resulting curve was
> converted to the exponential representation.

**Linear representation (Exponential)**
![11](https://user-images.githubusercontent.com/36266329/81301524-d790e680-9081-11ea-8f09-aa20e450f892.jpg)

**logarithmic representation**
![111](https://user-images.githubusercontent.com/36266329/81301642-fdb68680-9081-11ea-83fe-847e0cac5ef8.jpg)



After looking at the results, we realize that **the best model is the Artificial Neutral Network (MLPRegressor),** and it has the best score !

## Deaths
When searching for data for the **United States**, we obtained data for 60 days, starting on **2/3/2020,** and the number of dead was **6** and we assumed on the first day. The data ended on **30/4/2020**, today 60, and the number of dead **63856**.

We took data for **8 days** randomly for the final **test and evaluation stage**. After that we trained the different models, got a **final evaluation** and represented them with **score for each model**.

*The following figure represents the **curve for each model** in addition to the **score** obtained:*
> **Note:** The data were represented using two methods, the first is a
> **logarithmic representation** and the second is a **Linear representation
> (Exponential)**. The models were trained in both methods, and we chose
> the best among them for each model individually.
> - When looking at the Linear Regression curve, we used logarithmic representation of data when training it, and the resulting curve was
> converted to the exponential representation.

**Linear representation (Exponential)**
![22](https://user-images.githubusercontent.com/36266329/81301807-35bdc980-9082-11ea-96c9-c0a6f65731c6.jpg)

**logarithmic representation**
![252525555](https://user-images.githubusercontent.com/36266329/81301849-45d5a900-9082-11ea-9f63-5ffc4c769c01.jpg)


After looking at the results, we realize that **the best model is the Artificial Neutral Network (MLPRegressor),** and it has the best score !
