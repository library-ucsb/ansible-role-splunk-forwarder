# ansible-role-splunk-forwarder
Role is used to download the SplunkForwarder package for the RHEL/CentOS/AlmaLinux distributions, install the package, and then configure the SplunkForwarder to communicate with the Library Splunk server.  The role is used by the Ansible playbook in the https://github.com/library-ucsb/iac-vm-linux-config-management repository.

## Role Variables

| Name                                                  | Types/Values       | Description                                                                          |
| ------------------------------------------------------| -------------------|------------------------------------------------------------------------------------- |
| `config_splunk_forwarder`                             | Boolean            | Boolean check for whether the Splunkforwarder needs to be configured                 |
| `splunk_admin_user`                                   | String             | Username of splunk admin that communicates with the Splunk server                    |
| `splunk_admin_pass`                                   | String             | Password of splunk admin that communicates with the Splunk server                    |
| `splunk_deployment_server`                            | String             | Name of the Splunk server                                                            |
| `splunk_forwarder_download_url`                       | String             | URL of the Splunkforwarder package download                                          |
| `package_name_forwarder`                              | String             | Subdirectory location of the Splunkforwarder package in /opt/splunkforwarder         |
| `user_splunk`                                         | String             | Username of Unix user that will own the Splunkforwarder directories and files        |
| `dir_home_splunk`                                     | String             | Location of the installation directory                                               |
| `package_name_forwarder`                              | String             | Subdirectory location of the Splunkforwarder package in /opt                         |
| `splunk_server_port`                                  | String             | Port for management traffic with the Splunk server                                   |
| `splunk_indexer_port`                                 | String             | Port for server indexing and ingest with the Splunk server                           |

## Additional

Currently the https://github.com/library-ucsb/iac-vm-linux-config-management is broken, and so this role is not being used.  The IAC Ansible play will either need to be fixed or reverted back to a working version.
