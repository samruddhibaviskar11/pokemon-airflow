# pokemon-airflow

Automated end-to-end data pipeline: Downloading Pokemon
images with Bing API, classifying using a CNN model in python, and storing results on S3 via MinIO and Airflow, running on Dockerized EC2.

Technology Stack: Python, AWS S3, Bing APIs, MinIO, Airflow, YAML, Docker, Boto3

Steps to create the project
1.Run the yaml file command from airflow doc
2.Create a airflow-data folder
3.Create Dockerfile
4.Create local.json
5.Create requirements.txt
6.Run docker-compose up. This will create dags, plugins, logs folder
7.Move the logs folder to airflow-data folder
8.Create bing_image_download.py in dags
9.Create classification.py in dags
10.Add pokemon.h5 inside dags
11.Copy the airflow.cfg file from users/<username> /airflow directory and paste it in airflow-data folder.
12.Create images and process_dir folder in dags folder
13.Make the necessary changes in yaml file.
14.In airflow.cfg file, change the path from “c/<username>/”  to  “/opt/”
15.Run the project with “docker-compose up –build” command
