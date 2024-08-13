# sms_spam_detector
![Screenshot 2024-08-13 at 5 54 28 PM](https://github.com/user-attachments/assets/ef8602f0-be9d-4e29-a555-6075ad93e033)

## Duane Anglin

# Overview
Instructions:

	•	Refactor code from an SMS text classification solution into a function.
	•	Construct a linear Support Vector Classification (SVC) model within the function.
	•	Train the SVC model using the provided data.
	•	Create a Gradio app to host the application.
	•	Enable users to test text messages through the app.
	•	Provide feedback to users, indicating whether the text is classified as spam or not based on the model’s performance.​

Part 1: Create the sms_classification function in gradio_sms_text_classification.ipynb:

To create the sms_classification function in the gradio_sms_text_classification.ipynb file, start by assigning the text message column of the DataFrame to the features variable and the “label” column to the target variable. Then, split the data into training and testing sets with a 33% test size. Build a pipeline to transform the test set to match the training set, fit the model to the transformed training data, and return the model. After loading the SMSSpamCollection.csv into a DataFrame, call the sms_classification function with this DataFrame and store the result in the text_clf variable.

Part 2: Create the SMS Prediction Function:

To predict the classification of a new text message, use the sms_prediction function. Depending on the prediction, if the message is classified as “ham,” return the message stating that the text is not spam. If the message is classified as “spam,” return the message indicating that the text is spam.

# References
Chat GPT, Kalvin Anglin, Jaidev Kler, Solutions examples from class.
