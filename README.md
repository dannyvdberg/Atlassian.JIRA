## Atlassian JIRA 
Ansible rols which installs and configures a basic Atlassian JIRA Installation


#### Requirements & Dependencies
- Tested with Ansible 1.9.3 or higher
- Tested with Ubuntu 14.04
- Java 1.7.* or Java 1.8*
- MySQL, PostgreSQL, Oracle, MSS


#### Variables

```yaml
jira_versie: 6.4.11 								# Version of JIRA Installation
jira_user: jira 									# Server user that runs and stops JIRA
jira_installatie_directory: /opt/atlassian/jira 	# Default Installation Directory
jira_data_directory: /opt/application-data/jira 	# Default Data Directory

jira_backdoor_connector: "yes"  					# Enter and change yes when you want to use a backdoor connector
jira_proxy_name: "myjira.com" 						# Enter and change your proxyName
jira_proxy_port: "443" 								# Enter and change your proxyPort
jira_proxy_scheme: "https"							# Enter and change your proxyScheme
jira_path: "/mycompany"								# Enter and change  path if you want to use it
mysql_connector: "yes"								# Enter yes when you use MySQL as database

jira_memory_settings_mn: 1024 						# Edit value for a different memory settings		
jira_memory_settings_mx: 2048						# Edit value for a different memory settings
```


###Example Playbook
```yaml
---
 - hosts: webservers
   roles:
   - dannyvdberg.Atlassian-JIRA
```


###Author Information
- Author:		Danny van den Berg


###Feedback, bug-reports, requests, ....
Feedback is welcome! Please send a e-mail to ddvandenberg@gmail.com


