# Udacity coursework

## Some Python Standard Library modules

`os` works with operating system
  - getcwd()
  - chdir()
  - system()
  - dir(os)
  - help(os)
  - listdir()
  
`shutil` is higher level interface to os
  - copyfile()
  - move()

`glob` for making file lists from wildcard dir searches

`sys` handles command line args
  - sys.argv
  - sys.argc
  - argparse()
  
`re` provides regular expressions
  - findall()
  - sub()
  
`math` provides floating point math
  - cos()
  - log()
  
`random` provides you with random seeds
  - choice()
  - sample()
  - randrange()
  
`statistics` calculates statistical properties
  - mean()
  - median()
  - range()

`urllib.request`
  - urlopen()
`urllib.error` handles errors from urrlib.request

`smtplib` lets you send mail if you have a local server
  - SMTP()
  - sendmail()
  
`datetime` works with formatting dates and times
  - today()
  - date()

`time` is for working with unix timestamps
  - sleep()

`webbrowser` 

`zlib` allows compression
  - compress()
  - decompress()
  
`timeit` calculates performance timing
  - Timer()

`doctest` tests interactions
  - testmod()
  - testfile()

`unittest` supports unit tests with assert statements
  - test_upper()
  - test_isupper()
  - test_split()
  
`json` works with JSON-formatted data
  - dumps()
  - loads()
   
`pickle` serializes Python objects

`email` package manages email messages
  - smtplib module
  - poplib module
  - imaplib module
  - mailbox module
  - smtpd module
  
`sqlite3` creates a lightweight db with no server process
  - connect()
  - execute()
  - commit()

## Stdlib Python Dev Tools from Command Line

`pydoc` auto-generates documentation from comment headers

`2to3` applies fixers to port from Python 2 to 3

## Non-Stdlib Python Development Tools

`doxygen` is a cross-language documentation generator

`pandoc` converts from one file to another

`PyMongo` works with MongoDB

## Classes/Instances

## CSS

##### Positioning

`Static flow` is the `normal flow`.

`Relative flow` placed `after normal flow` relative to `position in normal flow.`.

`Absolute flow` placed `before normal flow` relative to `parent`.

`Fixed flow` placed `before normal flow` relative to `viewport`.


##### 

Parent size calculations ignore float children.

# Linux Server Setup Checklist

## Update the System 

`sudo apt-get update`

`sudo apt-get upgrade`

`sudo apt-get autoremove`

`sudo apt-get install finger`

## Create a New User 

`sudo adduser grader`

`usermod -aG sudo grader`

## Generate the Keypair 

`ssh-keygen -t rsa -b 4096`

`vim .ssh/authorized_keys`

`chmod 700 ~/.ssh`

`chmod 644 ~/.ssh/authorized_keys`

## Improve the Security

`sudo vim /etc/ssh/sshd_config`

```
Port 2200
PermitRootLogin no
PasswordAuthentication
```

`sudo service ssh restart`

`sudo ufw default deny incoming`

`sudo ufw default allow outgoing`

`sudo ufw allow 2200/tcp`

`sudo ufw allow 80/tcp`

`sudo ufw allow 123/tcp`

`sudo ufw enable`

## Test the Login

`ssh grader@courseserver -p 2200`

# Catalog Project Draft README

Server: 45.33.78.30 (Linode)

URL: <coming soon>

Installed Software: 

- libapache2-mod-wsgy-py3
- postgresql
- apache2
- git 
- nmap

Configurations: 

- See above for security

Third Party Resources

- man pages
- Stack Ovrflow
