# kafka data pipeline using python

**Prerequisites**
* This project uses Docker and docker-compose. View this [link](https://docs.docker.com/engine/install/ubuntu/) to install the docker engine and this [link](https://docs.docker.com/compose/install/) to install the docker-compose.

* In this pipline,I have created python virtual environment.You can use any version of python .It is upon you.

**Create Virtual Environment(env_kafka)**
```
python -m venv env_kafka      
```


**Activate  Environment**
```
 . env_kafka/bin/activate
```

 and install the required libraries by executing the following commands:

**Install Libraries**
```
 pip install -r requirements.txt
```


## Producing and consuming data to Kafka

1. Run the docker-compose.yml file:
        
        docker-compose -f docker-compose.yml up -d
2. Wait a moment while Docker downloads the images and for the services to start up.

3. Create the **producer**:
        
        python producer.py

4. Create the **consumer**:

        python consumer.py
  
   In the terminal, every message that the producer has published is displayed.
   
   Data is now being **produced** to and **consumed** from Kafka.
   
5. By going to the [Control Center](http://localhost:9021), the same data can be seen in a UI.
   

