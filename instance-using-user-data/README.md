# instance-using-user-data.yaml

Start a single instance after querying some basic inputs:

- Stack Name - name shown in your Orchestration overview for this stack
- Creation Timeout - timeout in minutes until Heat considers it as failed
- Password for user "u123456-user" - password of your openstack user
- Instance Size - dropdown to choose from
- Hostname - the name of your server instance
- Image Name - drop down to choose your OS version
- SSH Keypair Name - the name says it all - upload/create a keypair before launching the stack
- Private Network - drop down - choose the name of your project network
- External Network - name of the external network (ext01 on pluscloud open)

You will be able to login as user ubuntu (or debian if you choose Debian) on the IP shown in the Overview tab of your stack.

The user-data section will get the latest updates and install an nginx server.
