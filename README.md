
## PROBLEM STATEMENT
A health tech company 'BeHealthy', aims to connect the medical communities with millions of patients across the country. ‘BeHealthy’ has a web platform that allows doctors to list their services and manage patient interactions and provides services for patients such as booking interactions with doctors and ordering medicines online. Here, doctors can easily organise appointments, track past medical records and provide e-prescriptions. They provide medical services, prescriptions and online consultations and generate huge data day by day.

Let’s take a look at the following snippet of medical data that may be generated when a doctor is writing notes to his/her patient or as a review of a therapy that he or she has done.“The patient was a 62-year-old man with squamous cell lung cancer, which was first successfully treated by a combination of radiation therapy and chemotherapy.”
As you can see in this text, a person with a non-medical background cannot understand the various medical terms.

Suppose you have been given such a data set in which a lot of text is written related to the medical domain. As you can see in the dataset, there are a lot of diseases that can be mentioned in the entire dataset and their related treatments are also mentioned implicitly in the text, which you saw in the aforementioned example that the disease mentioned is cancer and its treatment can be identified as chemotherapy using the sentence.
But, note that it is not explicitly mentioned in the dataset about the diseases and their treatment, but somehow, you should build an algorithm to map the diseases and their respective treatment.

You should identify the Diseases and their respective treatments from the data and list them as in the form of a table like the one below

![image](https://user-images.githubusercontent.com/56822829/138415785-93dc11c0-dffe-4bc0-b939-15bb6600fb78.png)



## UNDERSTANDING THE DATA 
Four datasets have been provided to you
- train_sent
- test_sent
- train_label
- test_label

The train dataset is used to train your model, and the test dataset is used to evaluate the built model. 

![image](https://user-images.githubusercontent.com/56822829/138418215-7def6480-8db9-46a6-b4cf-9aec0d0d1eeb.png)

First lets understand the ‘train_sent’ and the ‘test_sent’ datasets. Here, you need to understand that each word in this dataset is provided in a single line. Moreover, there are blank lines given in the dataset that have been highlighted in the image given above. These blank lines indicate that a new sentence is starting from the next line onwards to the next blank line.

Now, let’s take a look at the next datasets that are named ‘train_label’ and ‘test_label’.

![image](https://user-images.githubusercontent.com/56822829/138418321-922a87cb-47a9-400f-aa16-e7034a755ec6.png)

There are three labels that have been used in this dataset: O, D and T, which are corresponding to ‘Other’, ‘Disease’ and ‘Treatment’, respectively. These labels correspond to each word that is available in the ‘train_sent’ and 'test_sent' datasets. So, there is one-to-one mapping of each label available in the 'train_label' and 'test_label' datasets with the words that are available in the 'train_sent' and 'test_sent' datasets, respectively.
