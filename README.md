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
 
