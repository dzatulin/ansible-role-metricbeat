##Ansible Role: Metricbeat
Role for installing and configuring Metricbeat on the Elastic Stack
## Requirements
Ansible version: 2.9
Centos 7/ Debian
## Dependencies
None
## Example Playbook
```
- hosts:  "{{ var }}"
  vars:
    metricbeat_kibana_hosts: localhost:5601

    metricbeat_output_elasticsearch_enabled: true
    metricbeat_output_elasticsearch_hosts:
      - "localhost:9200"
    metricbeat_username: elastic
    metricbeat_password: "1234567890"

  roles:
    - ansible-role-metricbeat
```
