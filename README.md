Aim - To create an ETL Pipeline in AWS Cloud to store data and produce insights in Power BI

Services used - Amazon Account, S3 Buckets, AWS Glue, Redshift, and Power BI

Steps

The important part of this project is to upload and store the data in AWS Cloud.
1. I have considered a housing dataset online. 
2. Log in to your Amazon account and create an S3 Bucket in any region.
3. Upload the file into the bucket created as below
   ![image](https://github.com/Roshinid03/Housing_Property_Dashboard/assets/150306520/7447707f-ad52-4905-a967-c8b9afbbed11)
4. Open AWS Glue from the console and create a classifier.
   Classifier helps in reading the data into a data source.
   ![image](https://github.com/Roshinid03/Housing_Property_Dashboard/assets/150306520/5607a056-ffbc-4b00-a18a-d10a35566c63)
5. Create the databases for both the bucket and the redshift cluster.
   ![image](https://github.com/Roshinid03/Housing_Property_Dashboard/assets/150306520/ac0ae109-e906-431c-b19f-5e59f3529023)

6. Create a Redshift cluster.
It may take some time to create the cluster. 
Create the authentication credentials while creating the cluster to access it using crawlers.
![image](https://github.com/Roshinid03/Housing_Property_Dashboard/assets/150306520/cbc2985e-8f19-4559-a8ad-2581c33aed6a)

7. Create a crawler for the S3 Bucket.

8. Create a connection to the redshift.
   ![image](https://github.com/Roshinid03/Housing_Property_Dashboard/assets/150306520/5258d330-d2f4-43a0-92c6-d0ad0510d4ec)
9. Create the table in the cluster using the Query Editor available in the Redshift cluster console.
SQL Query can be used in running the table and adding values to the table.

![image](https://github.com/Roshinid03/Housing_Property_Dashboard/assets/150306520/1c5e84ae-d4e7-4600-bb84-8377993d5921)

10. Create the crawlers for the redshift cluster.
![image](https://github.com/Roshinid03/Housing_Property_Dashboard/assets/150306520/f2f6dde8-933a-4e40-8936-bcce7408a9cb)

    
11.	When both the crawlers are ready, start creating Visual jobs in AWS Glue.
12.	Drag and drop the source, transform used, and the destination where data should be transferred.
13.	An automatic script will be produced after dragging the tabs onto the dashboard.
14.	Start the running the job. 
15.	When the job is successful, open Power BI.
16.	Import data by connecting the Power BI to the AWS Redshift Cluster using the plugins.
17.	Transform the data in Power BI Desktop and start building the visualization dashboard.
![image](https://github.com/Roshinid03/Housing_Property_Dashboard/assets/150306520/2c551e5f-10e0-421e-9187-2c0af0a1b21d)



