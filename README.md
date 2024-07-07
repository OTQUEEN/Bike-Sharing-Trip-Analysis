# Bike-Sharing-Trip-Analysis
# How Does a Bike-Share Navigate Speedy Success?

# Scope of Analysis
1. *Introduction*
2. *Business task*
3. *Prepare Data*
4. *Process Data*
5. *Analysis and Visualization*
6. *Summary of Analysis (findings)*
1. *Recommendation*

## 1.1 About the company
In 2016, Cyclistic launched a successful bike-share offering. Since then, the program has grown to a fleet of 5,824 bicycles that are geotracked and locked into a network of 692 stations across Chicago. The bikes can be unlocked from one station and returned to any other station in the system anytime.
Until now, Cyclistic’s marketing strategy relied on building general awareness and appealing to broad consumer segments. One approach that helped make these things possible was the flexibility of its pricing plans: single-ride passes, full-day passes, and annual memberships. Customers who purchase single-ride or full-day passes are referred to as casual riders. Customers who purchase annual memberships are Cyclistic members.

## 1.2 Statement of Problem
According to cyclistic’s finance analysts, Moreno, annual members are much more profitable than casual riders. Although the pricing flexibility helps Cyclistic attract more customers, Moreno believes that maximizing the number of annual members will be key to future growth. Rather than creating a marketing campaign that targets all-new customers, Moreno believes there is a very good chance to convert casual riders into members. She notes that casual riders are already aware of the Cyclistic program and have chosen Cyclistic for their mobility needs.

# 2 Business Task
This work seeks to address better understanding how Morena and her team would be able to design marketing strategies aimed at converting casual riders into annual members.

## 2.1 Pose questions
1. *How do annual members and casual riders use Cyclistic bikes differently?*
2. *Why would casual riders buy Cyclistic annual memberships?*
3. *How can Cyclistic use digital media to influence casual riders to become members?*

 * **NB:** For the purpose of our data information, we shall restrict our analysis to only question *1* above.

## 2.2 Stakeholders
* Lily Moreno - The Finance analyst
* Cyclistic marketing analytics team
* Cyclistic executive team

# 3 Preparing Data
## 3.1 About Dataset
The dataset was collected and organized by Cyclistic, a bike-share company in Chicago and it's made and available for public consumption under the Data Agreement license, [click here for more](https://divvybikes.com/data-license-agreement).

## 3.2 ROCCC analysis
1. **Reliable:** The data is not really 100% trusted as it's taking from a different site [link](https://divvy-tripdata.s3.amazonaws.com/index.html) rather than the cylistic site.
2. **Original:** The data is from a third party site, hence not orignal.
3. **Comprehensive:** The data contains enough data for our analysis. **Sample used : 2021 - 2022**
4. **Current:** Yes, the data is up to date
5. **Cited:** It cition is unknown

# 4 Data Processing
In this section, we shall define the tool(s) that will be deployed for the cleaning of the data.

We will be using the R and sql for our data cleaning.

## 4.1 Setting up tool environment

![image](https://github.com/OTQUEEN/Bike-Sharing-Trip-Analysis/assets/152812768/76401510-7ca9-44cc-b8ed-7df0f6599d23)
## 4.2 Loading files 
![image](https://github.com/OTQUEEN/Bike-Sharing-Trip-Analysis/assets/152812768/68b4254f-6262-4319-8184-50569ea6d6fb)
### 4.2.1 Data properties
![image](https://github.com/OTQUEEN/Bike-Sharing-Trip-Analysis/assets/152812768/3478ead3-c29c-48c0-a8ab-54702ff43617)

We will make some random checks of the column names and the structure of the data to find out if they have similar properties.

![image](https://github.com/OTQUEEN/Bike-Sharing-Trip-Analysis/assets/152812768/aa7cfba8-b0b9-4479-8c8e-ef34e69fdfe3)
Now we can observe that all the years has same data type except year 2020. We will will need to change this to chr to enable us merge all the data as single.

### Merging the two years data as single data
trip <- bind_rows(merge_21, merge_22)

### Data formating and cleaning
![image](https://github.com/OTQUEEN/Bike-Sharing-Trip-Analysis/assets/152812768/d57ac900-a0b2-4534-b7ad-b1c4824f3739)
![image](https://github.com/OTQUEEN/Bike-Sharing-Trip-Analysis/assets/152812768/b1e57b2b-8061-4607-aaa2-d6e9e5ebd1e4)

## changing data type for station_id and also checking if there is no missing entry on member_casual column
![image](https://github.com/OTQUEEN/Bike-Sharing-Trip-Analysis/assets/152812768/5cfc8d4e-a4a6-4570-8efc-1ed84073f21f)
![image](https://github.com/OTQUEEN/Bike-Sharing-Trip-Analysis/assets/152812768/18fdfa19-33ac-46d0-b248-f6711e383bb3)
![image](https://github.com/OTQUEEN/Bike-Sharing-Trip-Analysis/assets/152812768/5aef17ec-148c-4a5d-878d-9fd31cb62f74)
![image](https://github.com/OTQUEEN/Bike-Sharing-Trip-Analysis/assets/152812768/039806a5-5302-42fd-8bb2-b9363753c2bc)
![image](https://github.com/OTQUEEN/Bike-Sharing-Trip-Analysis/assets/152812768/aa4d7bf8-7731-43bc-929e-83963c206d3c)

![image](https://github.com/OTQUEEN/Bike-Sharing-Trip-Analysis/assets/152812768/d213202d-dd18-4caf-80da-88a5d56e2327)
![image](https://github.com/OTQUEEN/Bike-Sharing-Trip-Analysis/assets/152812768/c09ed6fd-2b8c-49b4-baed-b0947d813194)
![image](https://github.com/OTQUEEN/Bike-Sharing-Trip-Analysis/assets/152812768/04170ba0-caa5-4158-a9d3-ad3e660b41e8)
![image](https://github.com/OTQUEEN/Bike-Sharing-Trip-Analysis/assets/152812768/99542182-3c1e-44e6-8f9f-e44741b91690)
![image](https://github.com/OTQUEEN/Bike-Sharing-Trip-Analysis/assets/152812768/e44a8502-b50f-4bbd-9341-11f82730c3d6)
![image](https://github.com/OTQUEEN/Bike-Sharing-Trip-Analysis/assets/152812768/a0ffbfff-e0c0-417b-a2df-835b20b1f14e)

















