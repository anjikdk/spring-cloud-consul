# spring-cloud-consul

Reference link: https://howtodoinjava.com/spring-cloud/consul-service-registration-discovery

# Configuring Consul in Local workstation
Before starting the exercise, We need to first download, configure and run consul agent in localhost.

1. Download from Consul portal (https://www.consul.io/downloads). Choose particular package based on the operating System. Once downloaded the zip, we need to unzip it to desired place.
2. Start Consul Agent in local workstation – The Zip file that we have unzipped, has only one exe file called consul.exe. We will start a command prompt here and use below command to start the agent.
consul agent -server -bootstrap-expect=1 -data-dir=consul-data -ui -bind=192.168.6.1
3. Make sure you enter the correct bind address, it would be different depending on the LAN settings. Do a ipconfig in command prompt to know your IpV4 address and use it here.
4. Test whether Consul Server is running – Consul runs on default port and once agent started successfully, browse http://localhost:8500/ui and you should see a console screen
5. So we have configured consul in our local machine and consul agent is running successfully. Now we need to create clients and test the service registry and discovery part
6. We have created student-service and school-serivce

