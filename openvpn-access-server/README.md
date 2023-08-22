# openvpn-as.yaml

Deploys a OpenVPN Access Server with the following input:

- Stack Name - name shown in your Orchestration overview for this stack
- Creation Timeout - timeout in minutes until Heat considers it as failed
- Password for user "u123456-user" - password of your openstack user
- Instance Size - dropdown to choose from
- Image Name - drop down to choose your OS version
- SSH Keypair Name - the name says it all - upload/create a keypair before launching the stack
- Private Network - drop down - choose the name of your project network
- External Network - name of the external network (ext01 on pluscloud open)

You will be able to login as user ubuntu (or debian if you choose Debian) on the IP shown in the Overview tab of your stack.

You will find the initial password in the /var/log/cloud-init-output.log file.

Login with https://<your_floating_ip> and the login creds out of cloud-init-output.log. You will have to fine tune the network settings before use. For example the IP address unter Configuration / Network Settings which points initially to the private ip of the instance - not the public ip.

The OpenVPN Access Server is free to use up to 2 connections. If you need more or if you need support, please obtain a license at https://openvpn.net/access-server/.

This is just a simple example on how to deploy an application like the OpenVPN Access Server.
