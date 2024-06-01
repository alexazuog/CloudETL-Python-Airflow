# CloudETL-Python-Airflow
This repository contains an ETL pipeline project utilizing Python, Apache Airflow, and AWS services.
The pipeline is designed to extract data from various sources, transform it to meet analytical requirements, and load it into a data lake . The project demonstrates the integration of these technologies to build scalable and efficient data workflows.

### Key Features:

- Python: Core programming language for scripting and data transformation.
- Apache Airflow: Workflow orchestration tool to schedule and monitor ETL processes.
- AWS Services: Leveraging AWS S3, AWS EC2 for computing resource, data storage and processing.


![ETL Project (Open weather _S3)](https://github.com/alexazuog/CloudETL-Python-Airflow/assets/115574934/fb6f8f22-6143-460e-8cc7-0d1aa9fb1126)

#### Step 1
- Launched an  EC2 ( T2 small)  instance on AWS 
- Make sure it is accessible through ssh, http,https
- Edit the inbound rule in the security section to allow port 8080 (airflow) to access the instance

#### Step 2
Connected to the instance using EC2 CONNECT and ran the following commands
- Run sudo apt update 
- Run sudo apt install python3-pip 
- Install pandas and requests using pip
- Pip install pandas
- Pip install s3fs
- Pip install requests
- sudo apt install python3-venv
- python3 -m venv myenv
- source myenv/bin/activate 
- pip install apache-airflow  
- airflow standalone (initialize airflow and creates admin and password that allows you to log into the airflow UI)

#### Step 3 
- Create an IAM role that gives the EC2 permission to access AWS s3 bucket
- Write a Python script that extracts data using a GET request to the OpenWeatherMap API, then transforms the data, and finally loads it into AWS S3.



