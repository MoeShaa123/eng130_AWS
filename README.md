## What is cloud computing?
Cloud computing is the on-demand delivery of IT resources over the Internet with pay-as-you-go pricing. Instead of buying, owning, and maintaining physical data centers and servers, you can access technology services, such as computing power, storage, and databases, on an as-needed basis from a cloud provider like Amazon Web Services (AWS).

Amazon Web Services (AWS) is the world’s most comprehensive and broadly adopted cloud platform. AWS has significantly more services, and more features within those services, than any other cloud provider–from infrastructure technologies like compute, storage, and databases–to emerging technologies

![image](https://user-images.githubusercontent.com/106158041/199238202-115cf486-5243-4385-8449-a5b7edfb64ae.png)
## Benefits of cloud computing

* Trade fixed expense for variable expense – Instead of having to invest heavily in data centers and servers before you know how you’re going to use them, you can pay only when you consume computing resources, and pay only for how much you consume.

* Benefit from massive economies of scale – By using cloud computing, you can achieve a lower variable cost than you can get on your own. Because usage from hundreds of thousands of customers is aggregated in the cloud, providers such as AWS can achieve higher economies of scale, which translates into lower pay as-you-go prices.

* Stop guessing capacity – Eliminate guessing on your infrastructure capacity needs. When you make a capacity decision prior to deploying an application, you often end up either sitting on expensive idle resources or dealing with limited capacity. With cloud computing, these problems go away. You can access as much or as little capacity as you need, and scale up and down as required with only a few minutes’ notice.

* Increase speed and agility – In a cloud computing environment, new IT resources are only a click away, which means that you reduce the time to make those resources available to your developers from weeks to just minutes. This results in a dramatic increase in agility for the organization, since the cost and time it takes to experiment and develop is significantly lower.

* Stop spending money running and maintaining data centers – Focus on projects that differentiate your business, not the infrastructure. Cloud computing lets you focus on your own customers, rather than on the heavy lifting of racking, stacking, and powering servers.

* Go global in minutes – Easily deploy your application in multiple regions around the world with just a few clicks. This means you can provide lower latency and a better experience for your customers at minimal cost.

## SAAS, PAAS and IAAS

* SAAS(Software as a service) - Utilizes the internet to deliver applications, which are managed by a third-party vendor, to its users.

* PAAS(Platform as a service) - Provides cloud components to software while being used mainly for applications.

* IAAS(Infrastructure as a service) - Fully self-service for accessing and monitoring computers, networking, storage, and other services.

![image](https://user-images.githubusercontent.com/106158041/199240394-e9ea8323-602d-4c1e-8e89-9ae68f774e5c.png)

![image](https://user-images.githubusercontent.com/106158041/199240513-89b88b5e-157c-4476-978f-87511c59b2c5.png)

## CapEx vs OpEx

Capital expenditures (CapEx) are major purchases a company makes that are designed to be used over the long term.

Operating expenses (OpEx) are the day-to-day expenses a company incurs to keep its business operational.

CapEx is often more expensive and labor-intensive and often requires greater patience to reap rewards. 

OpEx is often cheaper and more flexible to incur. 

![image](https://user-images.githubusercontent.com/106158041/199243217-d4f421ec-0964-4b61-87e7-548cb3524fc6.png)

## Diagram

![cloud drawio](https://user-images.githubusercontent.com/106158041/199686868-20156f47-45fd-45c9-905c-1f31c5c1a68f.png)

- Create a key file `- sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv D68FA50FEA312927`
- `echo "deb https://repo.mongodb.org/apt/ubuntu xenial/mongodb-org/3.2 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-3.2.list`
-  Update and Upgrade - `sudo apt-get update -y` && `sudo apt-get upgrade -y`
-  Install MongoDB `- sudo apt-get install -y mongodb-org=3.2.20 mongodb-org-server=3.2.20 mongodb-org-shell=3.2.20 mongodb-org-mongos=3.2.20 mongodb-org-tools=3.2.20`
-  Check if its running - `sudo systemctl status mongod`
-  Open the config file - `sudo nano /etc/mongod.conf`
-  Check if its listening on port: 27017
-  Change the config file to allow access to everyone by changing bindIp to 0.0.0.0

## Disaster recovery plan

- In case something goes wrong, you are able to recover your data. Reliable and fast recovery of data loss.

- Amazon S3 is an object storage service that stores data as objects within buckets

- Benefits are High availability, High security and budget friendly

- Can be used to backup files, revisit old files (infrequent access), and you can host a static website
![s3 drawio](https://user-images.githubusercontent.com/106158041/199713359-91679118-06dc-45c2-8c6d-8fa7d2ad1a76.png)


