
## PROBLEM STATEMENT
A health tech company 'BeHealthy', aims to connect the medical communities with millions of patients across the country. ‘BeHealthy’ has a web platform that allows doctors to list their services and manage patient interactions and provides services for patients such as booking interactions with doctors and ordering medicines online. Here, doctors can easily organise appointments, track past medical records and provide e-prescriptions. They provide medical services, prescriptions and online consultations and generate huge data day by day.

Let’s take a look at the following snippet of medical data that may be generated when a doctor is writing notes to his/her patient or as a review of a therapy that he or she has done.“The patient was a 62-year-old man with squamous cell lung cancer, which was first successfully treated by a combination of radiation therapy and chemotherapy.”
As you can see in this text, a person with a non-medical background cannot understand the various medical terms.

Suppose you have been given such a data set in which a lot of text is written related to the medical domain. As you can see in the dataset, there are a lot of diseases that can be mentioned in the entire dataset and their related treatments are also mentioned implicitly in the text, which you saw in the aforementioned example that the disease mentioned is cancer and its treatment can be identified as chemotherapy using the sentence.
But, note that it is not explicitly mentioned in the dataset about the diseases and their treatment, but somehow, you should build an algorithm to map the diseases and their respective treatment.

You should identify the Diseases and their respective treatments from the data and list them as in the form of a table like the one below
![image](https://user-images.githubusercontent.com/56822829/138415785-93dc11c0-dffe-4bc0-b939-15bb6600fb78.png)

## DATASET
Four datasets have been provided to you
- train_sent
- test_sent
- train_label
- test_label

The train dataset is used to train your model, and the test dataset is used to evaluate the built model. There are three labels that have been used in this dataset: O, D and T, which are corresponding to ‘Other’, ‘Disease’ and ‘Treatment’, respectively.
