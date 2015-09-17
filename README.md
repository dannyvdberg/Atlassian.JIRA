## Atlassian JIRA by Avisi

Ansible rols which installs and configures a basic Atlassian JIRA Installation


#### Requirements & Dependencies
- Tested with Ansible 1.9.3 or higher
- Testen with Ubuntu 14.04


#### Variables

```yaml
jira_versie: 6.4.11
jira_user: jira
jira_installatie_directory: /opt/atlassian/jira
jira_data_directory: /opt/application-data/jira

jira_backdoor_connector: ja
jira_proxy_name: myjira.com
jira_proxy_port: 443
jira_proxy_scheme: https
jira_path: /mycompany
mysql_connector: ja

jira_memory_settings_mn: 1024
jira_memory_settings_mx: 2048

jira_url: http://www.atlassian.com/software/jira/downloads/binary/{{jira_tar}}
jira_tar: atlassian-jira-{{jira_versie}}.tar.gz
jira_installatie_versie: atlassian-jira-{{jira_versie}}-standalone
```


###Example Playbook
```yaml
---
 - hosts: webservers
   roles:
   - Avisi.JIRA
```


###Author Information
- Author:		Danny van den Berg
- Company:		Avisi


###Feedback, bug-reports, requests, ....
Feedback is welcome! Please send a e-mail to ddvandenberg@gmail.com


