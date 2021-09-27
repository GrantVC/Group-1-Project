# Group 1 Project
## Skin Lesion Detection

### What topic did we choose and why did we choose it?

Skin cancer detection based on lesion pictures is the topic we chose. Most people are affected in some way and at some point in their life by skin cancer or the question of if it’s cancer. Most people have a decent amount of sun exposure without the protection of sunscreen. Our objective is to train a model to analyze images of lesions, and accurately predict whether a lesion has the properties of cancer and if the person should seek medical follow-up.

### Communication Protocols:

1.	During class time
2.	Slack
3.	Scheduled zoom meetings
4.	We have exchanged emails and phone numbers for texting and quicker communication

### Data Source
Tschandl, Philipp, 2018, "The HAM10000 dataset, a large collection of multi-source dermatoscopic images of common pigmented skin lesions", https://doi.org/10.7910/DVN/DBW86T, Harvard Dataverse, V3, UNF:6:/APKSsDGVDhwPBWzsStU5A== [fileUNF]

### Resources
- Visual Data Storage: Amazon S3
- Database: PostgreSQL
- Languages: SQL, Python

### Database Utilization

The dataset includes a metadata spreadsheet and four spreadsheets containing pixel counts for the sample images.
  - ![image](https://user-images.githubusercontent.com/83254435/133031814-8f12f8e6-ceb9-41ed-ad26-154fc2361f18.png)
  - ![image](https://user-images.githubusercontent.com/83254435/133032037-62079814-8191-4fb4-af83-dcf6787781c4.png)

The four spreadsheets can be joined into a single document. For the sake of space, the ERD does not display all 785 columns for these csv files. However, the naming structure remains consistent throughout.
  - ![ERD](https://user-images.githubusercontent.com/83254435/133032192-a65346b6-0e47-4d41-9100-db98e9fc2aa2.png)
  - "image_id" primary key will correspond with the sample images used to train the model
    - ![image](https://user-images.githubusercontent.com/83254435/133032897-c36a3ad6-4f19-4b90-a20b-4151f02566e7.png)
 

### ML Model

Lesion Image Classification using Logistic Regression (Binary Classification)

Logistic regression uses a sigmoid function which is not linear.

Steps to follow:
- Import all necessary libraries, such as:

1. Numpy and Pandas are used for data handling and processing.
2. PyTorch and Torchvision contains ML functions.
3. Matplotlib used for visualizing the data.
4. Jovian saves code in jovian.ml platform.

Preparing the data: the code can be ran in Kaggle which makes processing the data easier since it is on the cloud and Kaggle hosts the data.

- Load the dataset
- Separate the x data and y data from the data, then set the shape of x and y.
- Put x and y in a pandas dataframe.
- Check the unique values and visualize it.
- Optimize the parameters to best fit the training data

- Train/Test dataset (works well with large samples)
*we expect the model to have a low accuracy since it contains random values. Where the accuracy is defined as the amount of numbers the model correctly predicts by total input images.

- Visualization of training dataset.
- Modeling (Logistic Regression using Scikit Learn)
- Compute the accuracy result.
 
Here is an article that uses data from Kaggle as well and it is about Image Classification using Logistic Regression on the American Sign Language MNIST, https://medium.com/@gryangalario/image-classification-using-logistic-regression-on-the-american-sign-language-mnist-9c6522242ddf
![image](https://user-images.githubusercontent.com/81715217/134830920-2ceceb57-4d03-496f-8abf-3dee82eb43ad.png)
