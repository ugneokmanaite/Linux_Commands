# Creating a vagrant machine

## 1. `Vagrant up` 

- Creating a vagrant machine

## 2. `Vagrant ssh` 

- To go into the virtual machine 

## 3. `sudo apt-get update` 

- To carry out all updates
- sudo is to run command as admin for ubuntu 
- apt gets package manager to install, update and upgrade packages 
- `sudo apt-get update -y` (automated)

**using these steps we have now created a DEV environment**

**exit command to exit the machine**

## 4. Creating a readme file

- `nano commands.md`

## 5. Installing on vagrant machine 

- `sudo su` : to access from root 
- `sudo apt-get install nginx` : to install web server
- `systemctl status nginx` : to check the status of the program

## 6. Now we need to launch nginx web server in our browser 

- go on git bash 
- `nano vagrant file` 
- add the private network IP address to launch nginx 


```
Vagrant.configure("2") do |config|

  config.vm.box = "ubuntu/xenial64"
# creating a virtual machine ubuntu

  config.vm.network "private_network", ip: "192.168.10.100"
# creating private ip to access our nginx server on the web from inside >


#redirecting the above to the specific web address
  config.hostsupdater.aliases = ["development.local"]

end
```

- `vagrant reload`


## Destroying vagrant

- `vagrant destroy` in **git bash**
