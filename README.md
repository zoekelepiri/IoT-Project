# IoT Platform Programming and Design for Urban Environment Condition Analysis
This project focuses on developing an IoT platform for analyzing urban environmental conditions using Node-RED. The platform retrieves data from environmental sensors located in various cities in Greece and provides real-time monitoring and analysis of temperature, humidity, air pressure, PM10, and PM2.5 levels.

# Location Selection
You can choose to deploy the Node-RED platform either on your local PC or on the FRED (Freeboard, Node-RED, and Data) cloud environment provided by Sense Tecnic. If you opt for the cloud deployment, you'll need to create a free account on the FRED platform to access Node-RED.

# Specifications and Steps
<b>A) Data Retrieval from Environmental Sensors</b>
- Select a location in Greece using the Sensor.Community platform.
- Use the "http request" node in Node-RED to call the Sensor.Community API and retrieve data from environmental sensors.
- Refer to the API documentation on GitHub for information on how to use and call the API.

<b>B) Sensor Data Processing</b>
- Parse the JSON response obtained from the API call using the "http request" node and return a parsed JSON object.
- Extract relevant sensor data such as temperature, humidity, air pressure, PM10, and PM2.5 levels from the JSON object.

<b>C) Real-time Visualization</b>
- Display real-time graphical representations of temperature, humidity, PM10, PM2.5, and air pressure vs. time in Node-RED.
- Utilize Node-RED's dashboard nodes to create visualizations for monitoring environmental conditions.
  
<b>D) Data Storage</b>
- Store sensor data (temperature, humidity, air pressure, PM10, PM2.5) in a SQLite database at regular intervals (not less than every 5-6 minutes).
- Use the "litedb" node in Node-RED to interact with the SQLite database and store sensor data.

<b>E) Data Analysis and Calculation</b>
- Develop JavaScript functions using the "function" node to calculate the average values of sensor data (temperature, humidity, etc.) over a 2-hour interval.
- Store the calculated average values in a separate table in the SQLite database.

# Getting Started
To get started with the project:
- Clone the repository to your local machine.
- Install Node-RED and any necessary dependencies.
- Set up the Node-RED environment and configure the flows according to the project requirements.
- Deploy the Node-RED flows and start monitoring environmental conditions.
  
# Conclusion
This project demonstrates the development of an IoT platform for analyzing urban environment conditions using Node-RED. By integrating data retrieval, processing, visualization, and storage capabilities, the platform enables real-time monitoring and analysis of environmental parameters in Greek cities.
Retrieve and display the average values in the Node-RED UI for monitoring.
