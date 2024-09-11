<html>

<h1>Wazuh-Server-Configuration</h1>
<br />
<br />
<br />
<br />
In this project we will be creating a Wazuh Server for its XDR and SIEM capabilities. We will be deploying Wazuh in our test environment on a Linux host with Ubuntu 22.04. Operating system and hardware requirements can be found at https://documentation.wazuh.com/current/quickstart.html
<br />
<br />
Installation
<br />
<br />
For the first step we will be using the CLI to install the components. We will be using the simplified version that automatically installs the indexer, server, and dashboard components.
<br />
<br />
	1. Open your CLI and use the command below to download and start the installation assistant. 
curl -sO https://packages.wazuh.com/4.8/wazuh-install.sh && sudo bash ./wazuh-install.sh -a













<html/>
