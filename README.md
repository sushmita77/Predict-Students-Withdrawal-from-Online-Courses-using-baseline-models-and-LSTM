# Predict-Students-Withdrawal-from-Online-Courses-using-baseline-models-and-LSTM

Data : OULAD Student data records the student demographics and their clickstream information with the Virtual Learning Platform.

There are four categories of results. This research aims to predict the students that will either continue the course or Withdraw from a course.
Hence, records from three categories are considered (Pass, Withdraw and Distinction). The Pass and Distinction will be combined as the Pass category.
This becomes a binary classification problem to predict whether students dropout from course or not.

The training dataset is imbalanced and has more data points related to the Pass Category. SMOTE method helps to overcome this issue by oversampling the instances for Withdraw category.

The student interactions with the online platform are recorded and will be analyzed weekly to predict the withdrawals.
It is important to identify the students that can withdraw a course in the early weeks of the course duration. 
Hence, it is necessary to perform the student analysis on a weekly basis. The date reported of accessing the materials needs to be mapped accordingly to respective week numbers.

![image](https://user-images.githubusercontent.com/13360000/112727966-ea700c00-8f1c-11eb-8dd9-463395e6294f.png)

![image](https://user-images.githubusercontent.com/13360000/112727974-f360dd80-8f1c-11eb-958c-0bd34b8ff337.png)
