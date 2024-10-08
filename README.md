<html>

<h1>Wazuh-Server-Configuration</h1>
<br />
<br />
<br />
<br />
In this project we will be creating a Wazuh Server for its XDR and SIEM capabilities. We will be deploying Wazuh in our test environment on a Linux container with Ubuntu 22.04. Operating system and hardware requirements can be found at https://documentation.wazuh.com/current/quickstart.html
<br />
<br />
<br />
<br />
<h2>Installation</h2>
<br />
<br />
For the first step we will be using the CLI to install the components. We will be using the simplified version that automatically installs the indexer, server, and dashboard components.
<br />
<br />
	1. Open your CLI and use the command below to download and start the installation assistant. 
<br />
curl -sO https://packages.wazuh.com/4.8/wazuh-install.sh && sudo bash ./wazuh-install.sh -a
<br />
<img src="https://github.com/Andyvillanueva9/Projectimages/blob/de33bd0c978913e50d04cf2bad41c30fa001ec39/Screenshot%202.jpg">
<br />
<br />
The assistant will run for some time and will return a summary once completed with the following information. This information will be used to log in to the dashboard. 
<br />
<br />
INFO: --- Summary ---
<br />
INFO: You can access the web interface https://wazuh-dashboard-ip:443
<br />
&nbsp;&nbsp; User: admin
<br />
&nbsp;&nbsp; Password: ADMIN_PASSWORD
<br /> 
INFO: Installation finished.
<br />
<img src="https://github.com/Andyvillanueva9/Projectimages/blob/1e17da5d84e856006c6f9b06e797348337c6ede3/Screenshot%203.jpg">
<br />
2. Next we will use the ifconfig command to find the local ip so we can access the Wazuh dashboard through a browser using the format in the summary https://0.0.0.0:443.
<br />
<img src="https://github.com/Andyvillanueva9/Projectimages/blob/f2616eaf5f1b7915eb3d6aeb3f3b54d4b6df7117/Screenshot%204.jpg">
<br />
<br />
3. You can log in using the user and password provided in the Summary of the installation. Once logged in you should see the overview page on the dashboard.
<br />
<img src=https://github.com/Andyvillanueva9/Projectimages/blob/1e24f8106fa634925712d3a24d9744d9007ffce9/Screenshot%205.jpg>
<br />
<br />
At this point the server is now installed and you are ready to start configuring groups for your agents. The agent can be deployed and hosts will be added to the default group if you have not created any but can be moved at a later time.

<html/>
