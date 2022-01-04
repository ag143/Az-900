### What is Internet of Things?
Internet of Things (IoT) is a network of internet connected devices (IoT Devices) embedded in everyday objects enabling sending and receiving data such as settings and telemetry

- Some IOT  devices are equipped with sensors that collect data.the purpose of connecting and exchanging data with other devices and systems over the internet.Some common sensors are :- 
Bar and QR code 
Temp and humidity
Infrared or light sensor


Example -- 
IoT was first implemented in 1970's ATMs (or cash machines). They're considered to be one of the first examples of the IoT being used in our society. 
 
Also Amazon ECHO is a example of IOT These devices can include multiple appliances that need to be connected for reasons including automation and real-time control of the device. 

**Mainly IoT involves 3 main concepts 
#### Things
The physical objects or things, such as industrial equipment, devices or sensors, that connect to the cloud persistently or intermittently.

#### Insights
Information collected by the things, which is analysed and turned into actionable knowledge either by people or AI.

#### Actions
The way people respond to those insights and connect them to their business, as well as the systems and tools they use.


- How cloud helps IoT ?
Cloud gives the support needed for IoT

## Azure Iot Hub
- Managed service for bi-directional communication
- Platform as a Service (PaaS)
- Highly secure, scalable and reliable
- Integrates with a lot of Azure Services
- Programmable SDKs for popular languages (C, C#, Java, Python, Node.js)
- Multiple protocols (HTTPS, AMQP, MQTT)

#### business use case -- 
- Update your IOT devices on the air 
- Use device-to-cloud telemetry data to understand the state of your devices and define message routes to other Azure services—without writing any code. In cloud-to-device messages, reliably send commands and notifications to your connected devices and track message delivery
 
## Azure IoT Central
- IoT App Platform - Software as a Service (SaaS)
- Use industry-specific app templates for retail, energy, healthcare, and government to get up and running quickly
- No deep technical knowledge required
- Service for connecting, management and monitoring IoT devices
- Highly secure, scalable and reliable
- Built on top of the IoT Hub service and 30+ other services

## Azure Sphere

- Secure end-2-end IoT Solutions
- Azure Sphere certified chips (microcontroller units - MCUs)
- Azure Sphere OS based on Linux
- Azure Sphere has built-in communication and security features for internet-connected devices

### business use case -- 

An example would be that of an ATM in comparison to a washing machine. When security is a critical consideration in your product's design, the best product option is Azure Sphere

If you merely want to connect to your remote devices to receive telemetry and occasionally push updates, and you don't need any reporting capabilities, you might prefer to implement Azure IoT Hub by itself

# Big Data

### What is Big Data?
Big Data is a field of technology that helps with the extraction, processing and analysis of information that is too large or complex to be dealt with by traditional software.

The three V’s rule
Big data typically has one of the following characteristics

#### Velocity - how fast the data is coming in or how fast we are processing it
Batch
Periodic
Near Real Time
Real Time
#### Volume - how much data we are processing
Megabytes
Gigabyte
Terabytes
Petabytes
#### Variety - how structured/complex the data is
Tables
Databases
Photo, Audio
Video, Social Media

## Azure Synapse Analytics
Big data analytics platform (PaaS)
Multiple components
- [] Azure Synapse is an enterprise analytics service that accelerates time to insight across data warehouses and big data systems. Azure Synapse brings together the best of SQL technologies used in enterprise data warehousing, Spark technologies used for big data, Data Explorer for log and time series analytics, Pipelines for data integration and ETL/ELT, and deep integration with other Azure services such as Power BI, CosmosDB, and AzureML.

## Azure HDInsight
Flexible multi-purpose big data platform (PaaS)
Multiple technologies supported (Hadoop, Spark, Kafka, HBase, Hive, Storm, Machine Learning)

## Azure Databricks
Big data collaboration platform (PaaS)
Unified workspace for notebook, cluster, data, access management and collaboration
Based on Apache Spark
Integrates very well with common Azure data services
