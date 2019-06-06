# ansible-ssm-agent
This playbook helps you to install SSM Agent on your AWS Instances.

AWS Systems Manager Agent (SSM Agent) is Amazon software that can be installed and configured on an Amazon EC2 instance, an on-premises server, or a virtual machine (VM). SSM Agent makes it possible for Systems Manager to update, manage, and configure these resources. The agent processes requests from the Systems Manager service in the AWS Cloud, and then runs them as specified in the request. SSM Agent then sends status and execution information back to the Systems Manager service by using the Amazon Message Delivery Service (service prefix: ec2messages).
If you monitor traffic, you will see your Amazon EC2 instances, and any on-premises servers or VMs in your hybrid environment, communicating with ec2messages.* endpoints. 
Please git clone this repository to your VM.
```
git clone https://github.com/NadiraSaip/ansible-ssm-agent.git
````
Next, 
```
cd ansible-ssm-agent/
```
In order to make changes in yaml files you have to create your own repository and copy paste my playbook content.  After you have done changes git commit and git push it. Run the below command to check errors. 
```` 
ansible-playbook ssm-agent.yaml --check
````
Fix the errors if any found then run the following;
```
ansible-playbook ssm-agent.yaml
```
Ta da! SSM-Agent is installed
