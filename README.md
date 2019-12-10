# ZulipInfrastructure
System Deployment and Benchmarking Assessment

# Deploy
To provision VM intances in the cloud, you just need to run the command:

`ansible-playbook playbook.yml -b -i inventory.gcp.yml -u [YOUR_USERNAME] -K`

# Teardown
To delete the created VM instances, you just need to run the command:

`ansible-playbook teardown.gcp.yml -b -i inventory.gcp.yml -u [YOUR_USERNAME] -K`
