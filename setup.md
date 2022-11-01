## Set up AWS VM

- The first step is to copy the PEM file into our .ssh folder in GitBash

- Once that is done, log in to AWS using your account

- Now you want to create a new instance using your key pair that you have stored in your ssh folder

- Ensure that you use Ubuntu 18 OS which is free tier eligible

- Create a new security group with Port 22 and Port 80 open. Ensure the SSH port can only be used with your IP address

- Now you can launch the instance, check it's running by clicking on instances

- To connect to your instance, tick the box and click connect on the top right

![image](https://user-images.githubusercontent.com/106158041/199291865-92e2a274-bcce-4ada-baed-f8eb5a4b3936.png)

- Now you want to copy the example code into the .ssh folder

- Once you are inside the VM, check you are using the correct OS with `uname -a`

- Run `sudo apt-get update -y` and `sudo apt-get upgrade -y`

- Next install `nginx` using `sudo apt install nginx -y`

- Once you visit you Public IP, this should show up


![Screenshot 2022-11-01 165057](https://user-images.githubusercontent.com/106158041/199290848-1cca8b12-ed29-4263-b703-428b94a00128.png)

## Reverse Proxy

- To set up reverse proxy, SSH into the VM, run `sudo apt-get update -y` and `sudo apt-get upgrade -y`

- Next install `nginx` using `sudo apt install nginx -y`

- To set up the reverse proxy, you first need to get in to the Nginx files.

- To do this, `sudo nano /etc/nginx/sites-available/default` into VM home folder

- Then where it says location, replace the comments with this:

        proxy_pass http://localhost:3000;
        proxy_http_version 1.1;
        proxy_set_header Upgrade $http_upgrade;
        proxy_set_header Connection 'upgrade';
        proxy_set_header Host $host;
        proxy_cache_bypass $http_upgrade;`

- Exit once you have done that, and then check the syntax with `sudo nginx -t`

- Run `sudo systemctl restart nginx` and you have set up the reverse proxy
