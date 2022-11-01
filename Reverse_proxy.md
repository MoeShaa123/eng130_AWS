
![image](https://user-images.githubusercontent.com/106158041/199291865-92e2a274-bcce-4ada-baed-f8eb5a4b3936.png)




![Screenshot 2022-11-01 165057](https://user-images.githubusercontent.com/106158041/199290848-1cca8b12-ed29-4263-b703-428b94a00128.png)

## To set up reverse proxy, SSH into the VM, run `sudo apt-get update -y` and `sudo apt-get upgrade -y`

## Next install `nginx` using `sudo apt install nginx -y`

## To set up the reverse proxy, you first need to get in to the Nginx files.

## To do this, `sudo nano /etc/nginx/sites-available/default` into VM home folder

## Then where it says location, replace the comments with this:

        proxy_pass http://localhost:3000;
        proxy_http_version 1.1;
        proxy_set_header Upgrade $http_upgrade;
        proxy_set_header Connection 'upgrade';
        proxy_set_header Host $host;
        proxy_cache_bypass $http_upgrade;`

## Exit once you have done that, and then check the syntax with `sudo nginx -t`

## Run `sudo systemctl restart nginx` and you have set up the reverse proxy
