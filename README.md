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
7. Then jenkins ask for the required software to install, it will be similar like
<img width="1037" alt="Screenshot 2023-08-12 at 7 11 25 PM" src="https://github.com/raghavgarg1996/Jenkins/assets/117148030/c37a8bb4-d469-4f0a-9f98-bcb6f179e969">
8. Once the installation is complete it asks for these details
<img width="1106" alt="Screenshot 2023-08-12 at 7 15 08 PM" src="https://github.com/raghavgarg1996/Jenkins/assets/117148030/c27389ed-8a91-4807-a263-701c4076483f">
9. Gave the username:**admin**, password:**admin**, Full name: **Jenkins Admin**, and hit save and contimue
10. Then it will show Jenkins URL: http://192.168.1.1:8080/ .
11. In order to stop the container use command **docker-compose down**, and it will delete all the data


**Creating First Jenkins Job**
1. Select the Project Type - Free Style
2. Add Build Steps - Execute shell
3. In shell container write code "echo HELLO_WORLD"