# PLEXIO---INTERNSHIP-PROJECT
PLEXIO is a small device used in factories to collect machine data like speed,temperature and pressure.
It works like a translator-it converts PLC machine data into internet data.
The data is sent to cloud using Amazon Web Services so managers can see it on a dashboards.
The system has 5 layers - Hardware,connection,protocol,data processing and cloud.
It supports different PLC types( Modbus,Omron,Siemens),but all use the same adapter interface.
Every second,it reads data,checks if it is valid,and stores it.
Data is always saved to disk first then send to the cloud.
If internet is down,data is stored and stored later when connection returns.
It uses worker threads so one slow machine does not affect others.
Alerts are sent through the cloud not directly from the device.
It is used by the factory managers,maintenance engineers and plant operators.
It makes it easy to monitor data in real time and gives alerts,helping prevent breakdowns and delays.
