
# <img src="/logo/tableu.png" width="200" />&nbsp;&nbsp;&nbsp;Tableu Dashboard Project

*This Project is the Capstone Project of [INSAID](https://www.insaid.co/). All data has been provided by [INSAID](https://www.insaid.co/).*
![Symbol](https://www.insaid.co/wp-content/uploads/2019/09/logohalfx.png)

---
## [`Go to project application`](https://telecom-dashboard-sj.herokuapp.com/)

\
[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/) 
[![Made withJupyter](https://img.shields.io/badge/Made%20with-Jupyter-orange?style=for-the-badge&logo=Jupyter)](https://jupyter.org/try)

---
---
## Project Description

### Company 
Insaid Telecom is one of the leading telecom players, understands that customizing offerings is very important for its business to stay competitive

### Problem Statement
Insaid Telecom has lodes of customer data which can be used to help the Brand Advertisers to increase the sales by focusing on the customer behavior in the different regions. We are going to study the demographics of a user (gender and age) based on their app download and usage behaviours. The Data is collected from mobile apps that use Inside Telecom services. Full recognition and consent from an individual user of those apps have been obtained.

### Solution
Create a dashboard to visualise data from several fields to address the issue. 

### Purpose:
- This project will help to their clients better understand and interact with their audiences.
- In this consulting assignment, we have prepared a dashboard based on the customer data collected by Insaid Telecom.
- This dashboard will help to understand a user’s demographic characteristics based on their mobile usage, geolocation and mobile device properties.

### Sources of Data 
- Events_data :
When a user uses mobile on an INSAID Telecom network, the event gets logged in this data.
Each event has an event id, location (lat/long), and the event corresponds to the frequency of mobile usage. timestamp: when the user is using the mobile

- Gender_Age_data :
This data is based on the gender, age and age group for the particular device ids

- Phone_Brand_device model data :
This dataset gives the information about the mobile phone brands and device models used by the particular user. Many phone brands are given by its Chinese names.

### *You can check all coding steps in jupyter notebook*

## **The dataset is merged into one using following code**
```python
#Events_data merged with Gender_Age_data
test_merge_1 = df.merge(df2, how = "inner", on = "device_id")

#Events_data merged with Phone_Brand_device model data
test_merge_2 = df.merge(df3, how = "inner", on = "device_id")

# All merged
test_merge_3 = test_merge_1.merge(test_merge_2[['device_id','phone_brand', 'device_model']], how = "left", on = "device_id")

# save Dataset
test_merge_3.to_csv('Final_Dataset.csv')
```

`
Please check Final_Dataset.csv
`

# [`Go to project application`](https://telecom-dashboard-sj.herokuapp.com/)
## 🔗 Connect Me
[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://github.com/ShubhamCJagtap)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/shubham-jagtap-scj4497/)
[![mail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:shubham.c.jagtap@gmail.com)
