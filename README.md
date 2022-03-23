# SRE Intro
## User Journey 
### User experience 
#### Cloud computing with AWS
##### AWS Services

- Creating github repo to push the markdown doc
- Amazon Web Services (AWS)
  
  
  
###  Benefits of Cloud Computing

- Ease of use
  
- Felxibility
   
- Robustness
  
- Cost
### Linux Command

- How to start a service `sudo systemctl start name_service`
- how to stop a service `sudo systemctl stop name_service`
- how to check status `systemctl status service_name`
- how to enable service `sudo systemctl enable service_name`
- how to install a package `sudo apt install package_name -y`
- how to remove a package `sudo apt remove package_name -y`
- how to check all process `top`
- who am i `uname` or `uname -a`
- where am i `pwd`
- create a dir `mkdir dir_name`
- how to check `ls` or `ls -a`
- how to create a file `touch name_file` or `nano file_name`
- how to check content of the file without going inside the file `cat file_name`

- how to move a file `move file.txt from current location to sre folder`
- how to delete folder `sudo rm -rf folder_name`
  
### File permisions 
- how to check a file permision `ll`
- change file permision `chmod required_permision file_name`
- write `w` read `r` exe `x`
- https://chmod-calculator.com/




### Bash scripting - Automate process with the script

- code block
```bash
# create a file called provision.sh

# it must start with #!/bin/bash
#!/bin/bash

# run updates
sudo apt-get update -y
# run upgrades
sudo apt-get upgrade -y

# install nginx
sudo apt-get install nginx -y      

# ensure it's running - start nginx
sudo systemctl start nginx

# enable nginx
sudo systemctl enable nginx

```

- change the file to exe `chmod +x provision.sh`
- how to run an exe file `./provision.sh`

