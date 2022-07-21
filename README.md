# DeployEC2AWSCli-RHELVersion

This repository contains a little `bash-script` to easily deploy any instance in aws ec2 using aws-cli.

## Details

This script can be used to deploy any EC2 RHEL version instance in aws ec2 using aws-cli.
At the moment the script creates a t2.micro instance of the free layer and uses the Official ALMALinux AMI ID to install an up-to-date and working debian system.

This script creates a standard security group with the basic rules for web access with the ports:
* 80
* 443
* and a custom SSH port that the user sets for security.

This script creates a pem key in the folder or place where you are located in your terminal:
> You can copy the file elsewhere to keep it in a safe place.
![PEMFile](https://raw.githubusercontent.com/lfelipe1501/lfelipe-projects/master/AWSCliUBNT/AWSCliUBNT.png)

It also creates a floating IP so that the machine is always connected to a Fixed IP.

All the resources assigned in this script are left with their own name that the script creates randomly.

> *This script does not ask for the region to deploy the instance, it assumes that you already have this configured in your aws-cli environment or if you are using cloudshell, that you are in the region where you want to deploy the new server.*

## How to use

Its use is very simple, you just need to go to the cloudshell in your aws console or configure and use aws-cli app on your favorite linux distro:

```bash
wget -qN https://raw.githubusercontent.com/lfelipe1501/DeployEC2AWSCli-RHELVersion/main/DeployAWS-RHLBase.sh && chmod +x DeployAWS-RHLBase.sh && bash DeployAWS-RHLBase.sh
```

a small example of how it works :sunglasses:

https://user-images.githubusercontent.com/7816653/180266731-b74b41b4-3b75-489c-b4ed-b1e6cc99e893.mp4

### that's it

### Contact / Social Media

*Get the latest News about Web Development, Open Source, Tooling, Server & Security*

[![Twitter](https://github.frapsoft.com/social/twitter.png)](https://twitter.com/lfelipe1501)
[![Facebook](https://github.frapsoft.com/social/facebook.png)](https://www.facebook.com/lfelipe1501)
[![Github](https://github.frapsoft.com/social/github.png)](https://github.com/lfelipe1501)

### Development by

Developer / Author: [Luis Felipe Sánchez](https://github.com/lfelipe1501)
Company: [lfsystems](https://www.lfsystems.com.co)

