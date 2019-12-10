# ZulipInfrastructure
System Deployment and Benchmarking Assessment

# Deploy
To provision VM intances in the cloud, you need to:
  * Go to the cloud project and get your credentials in JSON format;
  * Create a file in the project directory named 'credentials.json' and insert into it the cloud credentials;
  * Then you just need to run the following command:

`ansible-playbook playbook.yml -b -i inventory.gcp.yml -u [YOUR_USERNAME] -K`

# Teardown
To delete the created VM instances, you just need to run the command:

`ansible-playbook teardown.gcp.yml -b -i inventory.gcp.yml -u [YOUR_USERNAME] -K`
