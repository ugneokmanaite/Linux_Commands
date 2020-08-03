# Introduction to commands

## sudo apt-get update -y

- Where am I? pwd is the command to ind your current location!
- What do I have available in the current dir? ls command (ls -a for hidden files)
- How can I find out the name of the system I am using? uname command and - shows the name of the current OS in Linux ubuntu

- Who am I? - who command
- clear command will clear the current screen

## How can I create a file?
- touch nameoffile --> touch myfirstfile.txt

## Creating directory
- mkdir nameofdir --> mkdir myfirstdir

## To go inside the directory
- cd myfirstdir

## To autofill
- start typing & then press TAB!

## Saving files
- control + x 
- y + enter

## Navigating in Linux
- to go back a folder --> cd..
- to go back to home location --> cd + enter
- go inside folder --> cd / nameoffolder

## Deleting file
- rm nameoffile --> use sudo rn nameoffile if permission denied

## Changing to root user
- sudo su --> master user

## Checking who is using the machine 
- command id

## Printing on command line 
- echo "hello"

### Session Management

- ``` top ``` --> Show real time processes
- ``` killall name ``` --> Kill all the processes with that name
- ``` uname ``` --> Displays name of the Operating System
- ``` pwd ``` --> Shows Current File Location
- ``` sudo command ``` --> Runs the Command as Admin
- ``` sudo su ``` --> Changes To Root User
- ``` exit ``` --> Return Back To Normal User

### File Operations


- ``` touch filename ``` --> Create a file
- ``` nano filename ``` --> Enter a file
- ``` rm filename ``` --> Remove a file
- ``` file filename ``` --> Get type of file
- ``` head filename ``` Shows first 10 lines of file
- ``` tail filename ``` --> Shows last 10 lines of file

### File Permissions

- ``` chmod +x filename ``` --> Give executable permission to a file

### Bash Variables

- ``` env ``` --> Shows all the Environment Variables
- ``` name ="Andrew" ```
- ``` echo $name ``` --> Displaying the value of the variable
- ``` export name ="Andrew" ``` --> Making name an Environment Variable

### Bash Script Commands

- ``` > command ```  --> Redirects Output to a File
- ``` >> command ``` --> Redirects Output to a File and Appends Output To End Of File
e.g..

```
echo "server{listen 80;
  listen 80;
  location / {
      proxy_pass http://192.168.10.100.3000;
  }
}" >> reverse-proxy.conf
```

The command in the echo will be added into the file named 'reverse-proxy.config'