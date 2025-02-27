# PowerBI-MongoDB-Connection
Power BI MongoDB Connection – A step-by-step guide on connecting Power BI to a MongoDB database. 🚀 

## Prerequisites  

- **MongoDB** installed  
- **Power BI** installed  
- **MongoDB BI Connector** installed – [Download Here](https://www.mongodb.com/try/download/bi-connector)  
- **MongoDB ODBC Connector** installed – [Download Here](https://github.com/mongodb/mongo-bi-connector-odbc-driver/releases/)  

## Steps to Connect Power BI to MongoDB  

### 1. Run the MongoDB BI Connector (`mongosqld`)  

- Open **Command Prompt** and run:  
  ```shell
  "C:\Program Files\MongoDB\Connector for BI\2.14\bin\mongosqld.exe"
  ```  
- If you installed it in a different directory, update the path accordingly.  
- The server and port will be displayed in the terminal.


![1](images/1.png)


### 2. Configure ODBC Data Source  

- Click **Windows Key**, search for **ODBC Data Sources**, and open it.  
- Navigate to the **System DSN** tab and click **Add**.  
- Select **MongoDB ODBC ANSI Driver** and click **Finish**.  
- Fill in the following details:  
  - **Data Source Name (DSN)**: Choose any name.  
  - **Description**: (Optional)  
  - **Server & Port**: Use the values shown in the `mongosqld` terminal.  
- Click **Test Connection** → Ensure it shows **"Connection Successful"**.  
- Select the database and click **OK**. 


![2](images/2.png)


![3](images/3.png)


### 3. Connect Power BI to MongoDB  

- Open **Power BI Desktop**.  
- Click **Get Data** → Select **Other Sources** → Search for **ODBC**.  
- Click **ODBC** and then **Connect**.  
- Choose the **Data Source Name (DSN)** you created earlier.  
- Click **OK**, and **CHOOSE WINDOWS AND DON'T CHANGE ANYTHING IN THIS WINDOW AND CLICK CONNECT**. Power BI will connect to MongoDB.  
- You should now see your database and collections in Power BI.


![4](images/4.png)


![5](images/5.png)


![6](images/6.png)


![7](images/7.png)


## Confirmation  

 
  ![8](images/8.png)  

 
  ![9](images/9.png)  


## Troubleshooting Tips  

- Ensure `mongosqld` is running before connecting.  
- Check **firewall settings** if connection issues occur.  
- Use the correct **ODBC driver version** that matches your MongoDB setup.  

## Author  

[Aravind R](https://linkedin.com/in/arav-r) 
