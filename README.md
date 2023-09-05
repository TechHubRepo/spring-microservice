# spring-microservice
Welcome to Spring Microservice demo or sample application

# Setup
Follow the following steps to install application

	Step 1 : Update the system packages
		$ sudo apt-get update
		
	Step 2 : Install OpenJDK 17
		$ sudo apt install openjdk-17-jdk -y
		
	Step 3 : Install Maven
		$ sudo apt install maven -y
		
	Step 4 : Install Git
		$ sudo apt-get install git -y
		
	Step 5 : Clone as following
		$ git clone https://<access_token>@github.com/TechHubRepo/spring-microservice.git
			
	Step 6 : Install MySQL 8
		• Update system repositories
			◦ $ sudo apt-get update
		• Install mysql
			◦ $ sudo apt install mysql-server -y
		• Verify the MySQL
			◦ $ mysql –version
		• Install MySQL Security
			◦ $ sudo mysql_secure_installation -y
			◦ Password : Password123#@!
			◦ If the terminal ask you to set the default password using ALTER statement then close the terminal and open again
				$ sudo mysql
				ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'Password123#@!';
				FLUSH PRIVILEGES;
			  Note : The MySQL Server will automatically started when you start system.
		• Create the following user (Optional)
			◦ CREATE USER 'myAdmin1'@'localhost' IDENTIFIED BY 'Password123#@!';
		• To Login next time with password
			◦ $ mysql --user='root' --password;
			◦ $ mysql --u='root' --p;

# How to Run
Goto project cloning directory and use any of following option to run the application

	Option 1
		$ mvn spring-boot:run
	Option 2
		Step 1 :  $ mvn clean compile package
		Step 2 :  $ java -jar target/<file-name>.war

