# HW1: Predicting Car Price
The dataset is look like this
![image](https://github.com/Tonpattra/Machine-Learning/assets/89975216/fbdf466b-0b33-4c6b-a244-c57194895dfe)

## Task 1 :Preparing the datasets 
- Download the Car Price dataset from Google classroom. Perform
loading, EDA, preprocessing, model selection, · · · , inference. Grade will be given based on the how well
you adhere to best practices. There are some important coding considerations:

- For the feature owner, map First owner to 1, ..., Test Drive Car to 5
- For the feature fuel, remove all rows with CNG and LPG because CNG and LPG use a different
mileage system i.e., km/kg which is different from kmfeaturepl for Diesel and Petrol
- For the feature mileage, remove “kmpl” and convert the column to numerical type (e.g., float).
Hint: use df.mileage.str.split
- For the feature engine, remove “CC” and convert the column to numerical type (e.g., float)
- Do the same for max power
- For the feature brand, take only the first word and remove the rest
- Drop the feature torque, simply because Chaky’s company does not understand well about it
- You will found out that Test Drive Cars are ridiculously expensive. Since we do not want to
involve this, we will simply delete all samples related to it.

Show the results in Task 1:
![image](https://github.com/Tonpattra/Machine-Learning/assets/89975216/1a876cff-1ece-43ad-bab9-b6d89dbe2e39)


## Task 2 :Report 
- In the end of the notebook, please write a 2-3 paragraphs summary deeply discussing
and analysing the results. Possible points of discussion:
- Which features are important? Which are not? Why?
  Ans: The feature are important are max_power, engine and years.you can check the the best feature form ppscore table in below: hight score means very important feature more than low score.
  
  ![image](https://github.com/Tonpattra/Machine-Learning/assets/89975216/f94e3b93-f1d1-47e6-807f-7b2f0f64c16e)
  
- For the feature fuel, remove all rows with CNG and LPG because CNG and LPG use a different
  Ans: I try to compare 4 model (algorithm_names = ["Linear Regression", "SVR", "KNeighbors Regressor", "Decision-Tree Regressor", "Random-Forest Regressor"]) Algorithm is perform well is  Random-Forest Regressor Because this model have the best Mean Score: -0.05946266469462726
  
  ![image](https://github.com/Tonpattra/Machine-Learning/assets/89975216/a4f21d99-6fbf-4bdc-8c18-5d8542759b1c)
  
## Task 3 :Deployment 
- Develop a web-based application that contains the model. Here you will be tasked to self-study how to deploy the model into production. Here are some guidelines:
- Here you have multiple options. Those who are veteran web developer may prefer their own web app
stack which is welcomed.
  - Users enter the domain on their browser. They land on your page.
  - (optional) Users may need to navigate to a prediction page.
  - Users read the instruction given on the page that instructs them on how the prediction works.
  - Users find the input form, put in the appropriate data, and click submit.
  - Note that if users do not have information on certain field, you have to allow users to skip that field.In that case, we recommend you to fill the missing field with imputation technique you have learned in the class.
  - A moment later (depending on your model and hardware performance), the result is returned and
printed below the form.

## Results :How to use Applications
This is the working window of the Application you will notice. upper right corner There are 5 details: main page, homework details page, results page, question page, contact page. And the last page is External.
![image](https://github.com/Tonpattra/Machine-Learning/assets/89975216/787550fc-08df-4786-bdab-2bf91f4bfdbf)

The results for Predicting Car Prices are available on the results page.
You can add data 3 type (power, engine and years)
![image](https://github.com/Tonpattra/Machine-Learning/assets/89975216/31abbfa9-d2f2-423b-b62b-32b4267619d7)

After that you can click send, Get the Data Received
![image](https://github.com/Tonpattra/Machine-Learning/assets/89975216/dd613bef-17d8-4399-8abb-42d28eb5ad9a)

And when you need to come back homepage, you cilck Button Back to homework
But you forgot to fill in one of the fields. there is no need to worry Because we will take the middle value of the data to Predict instead.

## Conclusion :
- I tried to write an application for the first time. I really like it and I feel very understanding in class. Thank you for the homework this time. That makes it a good experience!!
