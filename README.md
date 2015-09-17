## Atlassian JIRA by Avisi

Ansible rols which installs and configures a basic Atlassian JIRA Installation


#### Requirements & Dependencies
- Tested with Ansible 1.9.3 or higher
- Testen with Ubuntu 14.04


#### Variables

```yaml
jira_versie: 6.4.11 								# Version of JIRA Installation
jira_user: jira 									# Server user that runs and stops JIRA
jira_installatie_directory: /opt/atlassian/jira 	# Default Installation Directory
jira_data_directory: /opt/application-data/jira 	# Default Data Directory

jira_backdoor_connector: ja  						# Enter yes when you want to use a backdoor connector
jira_proxy_name: myjira.com 						# Enter your proxyName
jira_proxy_port: 443 								# Enter your proxyPort
jira_proxy_scheme: https							# Enter your proxyScheme
jira_path: /mycompany								# Enter a path if you want to use it
mysql_connector: yes								# Enter yes when you use MySQL as database

jira_memory_settings_mn: 1024 						# Edit value for a different memory setting			
jira_memory_settings_mx: 2048						# Edit value for a different memory settin
```


###Example Playbook
```yaml
---
 - hosts: webservers
   roles:
   - dannyvdberg.Atlassian.JIRA

   sudo: yes
```


###Author Information
- Author:		Danny van den Berg
- Company:		Avisi


###Feedback, bug-reports, requests, ....
Feedback is welcome! Please send a e-mail to ddvandenberg@gmail.com


