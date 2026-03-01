![](https://i.imgur.com/waxVImv.png)
### [View all Roadmaps](https://github.com/nholuongut/all-roadmaps) &nbsp;&middot;&nbsp; [Best Practices](https://github.com/nholuongut/all-roadmaps/blob/main/public/best-practices/) &nbsp;&middot;&nbsp; [Questions](https://www.linkedin.com/in/nholuong/)
<br/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=24&pause=1000&color=F7931E&width=435&lines=Hello%2C+I'm+Nho+Luong🇻🇳🇻🇳🇻🇳🇻🇳🇻)](https://git.io/typing-svg)

# **About Me🇻**
- ✍️ Blogger
- ⚽ Football Player
- ♾️ DevOps Engineer
- ⭐ Open-source Contributor
- 😄 Pronouns: Mr. Nho Luong
- 📚 Lifelong Learner | Always exploring something new
- 📫 How to reach me: luongutnho@hotmail.com

![GitHub Grade](https://img.shields.io/badge/GitHub%20Grade-A%2B-brightgreen?style=for-the-badge&logo=github)
<p align="left"> <img src="https://komarev.com/ghpvc/?username=amanpathak-devops&label=Profile%20views&color=0e75b6&style=flat" alt="amanpathak-devops" /> </p>

# ELK Stack Setup Step by step in Linux

=========================
## Downloading:

* ### Elasticsearch: https://www.elastic.co/downloads/elasticsearch

* ### Kibana: https://www.elastic.co/downloads/kibana

* ### Logstash: https://www.elastic.co/downloads/logstash

* ### Java: https://www.oracle.com/java/technologies/downloads/

## Note:
* * #### For elasticsearch version 8.12 you need to install Java version 21


## Moving the files

### The files will be in Downloads you need to move it to Ubuntu.

To do that follow this step:

Change the directory to Downloads first and then run this:

``` 
=> cd /mnt/c/Users/(username)/Downloads

Move the tar files to Ubuntu:

=> sudo mv (name-of-the-files) /home
```


## Extracting:

Change directory to Ubuntu:
```
=> cd /home

Then extract them:

=> sudo tar -xzvf (name-of-the-files)
```

## Configure Environment Variables:

```
=> nano ~/.bashrc
```

Add this below and save them (Ctrl + S) and exit (Ctrl + X).
```

export JAVA_HOME=/home/jdk-21.0.2

export PATH=$JAVA_HOME/bin:$PATH
```

Now to run them in Ubuntu we need to grant permissions:

```
=> sudo chown -R nholuong:nholuong /home/(kibana-8.12.0) OR (elasticsearch-8.12.0) OR (logstash-8.12.0)
```

* * ### Here, ```nholuong``` is the username.

To add a new user, run this:
```
sudo adduser (username) 

Then run the above line.
```


## Few steps to do before running the elk-stack:

### Generate Kibana Enrollment Token:

In a new terminal, navigate to the Elasticsearch bin directory:

```
=> cd path/to/elasticsearch/bin
```

Run the command:
```
=> ./elasticsearch-create-enrollment-token --scope kibana
```
* * ### Copy and save the generated token.

## Enter Enrollment Token in Kibana:

Paste the enrollment token into the Kibana configuration interface in your browser.


### Reset Elasticsearch Password:

In a new terminal, navigate to the Elasticsearch bin directory.

Run the password reset command:
```
=> ./elasticsearch-reset-password -u elastic
```

* ### Note down the newly generated password.


## Running the stack:

For elasticsearch go to this directory:

```
=> cd /home/elasticsearch-8.12.0/bin
```
Then run this:
```
=> ./elasticsearch
```

For kibana go to this directory:

```
=> cd /home/kibana-8.12.0/bin
```
Then run this:
```
=> ./kibana
```

### You might encounter an error when running Kibana, try this:

```
=> sudo ./kibana --allow-root
```

* ### (P.S. This error only came once for me)

For logstash go to this directory:

```
=> cd /home/logstash-8.12.0
```
Then run this:
```
=> bin/logstash -e 'input{stdin{}} output{stdout{}}'
```

![](https://i.imgur.com/waxVImv.png)
# I'm are always open to your feedback🚀
# **[Contact Me🇻]**
* [Name: Nho Luong]
* [Telegram](+84983630781)
* [WhatsApp](+84983630781)
* [PayPal.Me](https://www.paypal.com/paypalme/nholuongut)
* [Linkedin](https://www.linkedin.com/in/nholuong/)

![](https://i.imgur.com/waxVImv.png)
![](Donate.png)
[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/nholuong)

# License🇻
* Nho Luong (c). All Rights Reserved.🌟
