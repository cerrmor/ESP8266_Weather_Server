# ESP8266_Weather_Server
This project is about creating a secure local IoT weather station that is accessible to be monitored from anywhere. 

Security Concerns
* How to safely expose the esp8266 weather server to the internet
* How to protect against DoS attacks
* How to control exposed information
* How to prevent unwanted changes or injections of malicious code (firewall protection)
* Input validation
* Buffer overruns

Possible Secure Design
* Relay esp8266 through a protected sever using MQTT connection
* Use VPN client to obfuscate connection information
* Use reverse proxy for handling authentication
* Use a service like firebase for handling authorized connections

Priority step
Establishing Security protocols
* Use Wi-Fi manager to avoid hard coding Wi-Fi credentials

Secondary step
Building the weather server
First task
* Create a basic server and test local functionality
  * Add esp8266 Async library to code
  * Initialize Async connectivity to allow multi connection service
  * Initialize very basic webpage response
  * Upload to esp8266 and test output

Second task
* Connect embedded sensor unit to microcontroller
  * Connect wires to sensor
  * Add sensor library to code
  * Add sensor outputs to serial output for initial testing of data output
  * Upload to esp8266 and test

Third task
* Update webpage to display sensor readout
  * Update sensor out put in real-time

Fourth Task
* Update the webpage output to be pretty