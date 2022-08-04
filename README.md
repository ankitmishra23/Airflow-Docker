# Airflow-Docker

Airflow 2.3.0 with Docker

### Install Spark on 1 Airflow Worker

- Execute following docker command- `docker exec -u 0 -it <containerid> /bin/bash`
  <strong>Install Java</strong>
  - use following commands
    - `sudo apt-get update`
    - `sudo apt install openjdk-11-jdk`
    - check `java -version`
- Install python if not present. `sudo apt install python3`
  <strong>Spark Installation</strong>
- Navigate to tmp
- Download spark tar file from apache.org using wget. `wget https://dlcdn.apache.org/spark/spark-3.3.0/spark-3.3.0-bin-hadoop3.tgz .`
- Unzip spark tar file. `tar -xzf spark-3.3.0-bin-hadoop3.tgz`
- Move it to home and delete tar file. `mv spark-3.3.0-bin-hadoop3 ../home/spark ` and ` rm spark-3.3.0-bin-hadoop3.tgz`
- Navige to home directory
- Set Environment variable.
  - `export SPARK_HOME=/home/spark`
  - `export PATH=$PATH:$SPARK_HOME/bin`
- check `spark-shell`
