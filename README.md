# Predict-Students-Withdrawal-from-Online-Courses-using-baseline-models-and-LSTM

Data : OULAD Student data records the student demographics and their clickstream information with the Virtual Learning Platform.
Data Files Used : studentInfo.csv, studentVle.csv, vle.csv

This project aims to predict the students that will either continue the course or Withdraw from a course.
There are four categories of results. Hence, records from three categories are considered (Pass, Withdraw and Distinction). 
The Pass and Distinction will be combined as the Pass category. This becomes a binary classification problem to predict whether students dropout from course or not.

The training dataset is imbalanced and has more data points related to the Pass Category. SMOTE method helps to overcome this issue by oversampling the instances for Withdraw category.

The student interactions with the online platform are recorded and will be analyzed weekly to predict the withdrawals.
It is important to identify the students that can withdraw a course in the early weeks of the course duration. 
Hence, it is necessary to perform the student analysis on a weekly basis.
The date reported of accessing the materials needs to be mapped accordingly to respective week numbers.

![image](https://user-images.githubusercontent.com/13360000/112727966-ea700c00-8f1c-11eb-8dd9-463395e6294f.png)

![image](https://user-images.githubusercontent.com/13360000/112727974-f360dd80-8f1c-11eb-958c-0bd34b8ff337.png)

LSTM expects the training data in [samples, time steps, features] format.

As the main objective of this research is prior identification of dropouts the time steps are kept low ( 5 ,10 ,15 weeks).

The clickstreams arranged in a multidimensional format are the input to the LSTM model. The clickstreams across 20 different VLE materials will be used as the features and for every student data is maintained across all the 38 weeks.

Thus the 3D data expected by LSTM illustrates that for all students we have per student 38 weeks and 20 resources.

Lastly, a Merge Model will be created using the Functional API that will be comprised of the:

    1)Feed-Forward Neural Network and the 
    2)Long Short Term Memory
    3

![image](https://user-images.githubusercontent.com/13360000/112753460-9a9e4d00-8fcf-11eb-97e4-16ae5cff7837.png)
![image](https://user-images.githubusercontent.com/13360000/112753514-b0ac0d80-8fcf-11eb-9405-d06d2cd70a49.png)


