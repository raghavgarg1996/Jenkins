# Jenkins
Implementing jenkins and all it's test in thisrepo


**Pre-requisites**
1. Install docker
2. Install docker-compose


**Installation**

1. Go to jenkins-data folder.
2. Execute **docker-compose up -d** command
3. Once jenkis installation is done, execute command **docker logs -f jenkins**
4. In the logs seection will see hash something like this 338a54e407f***********
5. Now get your system ip and implement 8080 in it i.e
    192.168.1.1:8080 and hit the url.
6. Now paste the hash which we get in step 4 into the "**Administrator Password**"
7. Then jenkins ask for the required software to install
