# ansible-role-splunk-forwarder
Role is used to download the SplunkForwarder package for the RHEL/CentOS/AlmaLinux distributions, install the package, and then configure the SplunkForwarder to communicate with the Library Splunk server.

## Secrets


## Role Variables

| Name                                                  | Types/Values       | Description                                                                          |
| ------------------------------------------------------| -------------------|------------------------------------------------------------------------------------- |
| `splunk_admin_user:`                                  | String             | Username of splunk admin that communicates with the Splunk server                    |
| `splunk_admin_pass:`                                  | String             | Password of splunk admin that communicates with the Splunk server                    |
| `splunk_deployment_server`                            | String             | Name of the Splunk server                                                            |
| `splunk_forwarder_download_url`                       | String             | URL of the Splunkforwarder package download                                          |
| `package_name_forwarder`                              | String             | Subdirectory location of the Splunkforwarder package in /opt/splunkforwarder         |
| `user_splunk`                                         | String             | Username of Unix user that will own the Splunkforwarder directories and files        |
| `dir_home_splunk`                                     | String             | Location of the installation directory                                               |
| `package_name_forwarder`                              | String             | Subdirectory location of the Splunkforwarder package in /opt                         |
| `splunk_server_port`                                  | String             | Port for management traffic with the Splunk server                                   |
| `splunk_indexer_port`                                 | String             | Port for server indexing and ingest with the Splunk server                           |

