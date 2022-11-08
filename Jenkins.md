### CI/CD

- The "CI" in CI/CD always refers to continuous integration, which is an automation process for developers. Successful CI means new code changes to an app are regularly built, tested, and merged to a shared repository.

- The "CD" in CI/CD refers to continuous delivery and/or continuous deployment, which are related concepts that sometimes get used interchangeably. Both are about automating further stages of the pipeline.

- A CDE (Common Data Environment is a cloud-based space where information from construction projects is stored and accessible to project participants

- The difference between continuous delivery and continuous deployment is the presence of a manual approval to update to production. 

- Webhooks are automated messages sent from apps when something happens. They have a message—or payload—and are sent to a unique URL—essentially the app's phone number or address.

![image](https://user-images.githubusercontent.com/106158041/200534633-ec4bbdd8-0c79-47c5-a2c0-9b4c348cfc7f.png)

### Jenkins

- Jenkins is an open source automation server. It helps automate the parts of software development related to building, testing, and deploying, facilitating continuous integration and continuous delivery.

- Many top companies are using Jenkins such as FaceBook, Netflix and LinkedIn because of its benefits.

- There are many other CI/CD tools you can use other than Jenkins such as TeamCity, Bamboo and GitLab.

![image](https://user-images.githubusercontent.com/106158041/200536000-e0d3b80b-b5bb-4ce1-99c1-affedfe1df9e.png)

### Benefits of Jenkins

- It is an open-source tool with great community support.
- It is easy to install.
- It has 1000+ plugins to ease your work. If a plugin does not exist, you can code it and share it with the community.
- It is free of cost.
- It is built with Java and hence, it is portable to all the major platforms.

### Steps

- Create a new ssh pair 
- Copy the public and private key into ssh folder
- Create a new CI/CD pipeline - app folder 
- Generate a new ssh pair (ensure to generate it in .ssh folder on localhost)
- Copy file.pub to github repo (will show you in a minute)
- Copy the private key in Jenkins

