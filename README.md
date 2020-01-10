# Ansible-practice

playbook for aws ec2 and s3

### <i>BUG</i>

- ec2_key module region unresolve

### TODO

### - ec2:

  [OK]  - create    (plain instance, LAMP server)

  [OK]  - terminate (with keypair deletion)

  [OK]  - start

  [OK]  - stop

  
- group of ec2 control: (hardcode instacnes id to var)
 
  [OK]  - start instances 
  
  [OK]  - stop instances
  
  [  ]  - control by tag
  
  [  ]  - control by group

### - s3:

  https://docs.ansible.com/ansible/latest/modules/s3_bucket_module.html#s3-bucket-module

  [OK]  - create bucket (bucket name must be universially unique)

  [OK]  - delete bucket
  
  [OK]  - GET
  
  [OK]  - PUT
  
  [OK]  - CORS
  
  [  ]  - lifecycle rule
  
  [OK]  - logging
  
  [OK]  - s3_sync (multiple files upload)
  
  [  ]  - configure bucket as website (static hosting)
  
### - Zabbix:

  https://docs.ansible.com/ansible/latest/modules/list_of_monitoring_modules.html#zabbix
  

### - Other basic functions:
  
  - Run command on remote node [command.yml]
