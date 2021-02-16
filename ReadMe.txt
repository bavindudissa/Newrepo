Instruction to setup the dev environment
1. Install Java 13
2. Install Apache Netbeans IDE 11.3 https://netbeans.apache.org/download/nb113/nb113.html
3. Install MySQL Workbench 8.0 CE  https://dev.mysql.com/downloads/installer/

Setup the database and table
1. Open MySQL Workbench
2. Execute the following query to create the database and table.
	Create database ReadFile;
	use Readfile;
	create table Email_Infor(
		Id int not null auto_increment,
		Email varchar (50) not null,
		Subject varchar (100),
		Message varchar (10000),
		Send_Date_Time datetime ,
		Send_Status varchar (15),
		primary key (Id)
	);

Open project using Netbeans IDE
1. Open Netbeans IDE
2. To add project to Netbeans use the following steps
	Go to File -> Open Project -> File Path of ReadText_SendEmail project folder -> Click on Open Project 
	Then you will be able to see the ReadText_SendEmail project folder inside Projects tab (left side of the IDE) 
3. Add require libraries to the netbeans project
	i.  Go to the Projects tab and click on the + sign of ReadText_SendEmail project
	ii. Then write click on the Libraries -> Click on Add JAR/Folder -> Add all the jar files inside the Java Libraries folder (Attached)
	
	
**** Before run the program please change the below sections accordingly
1. Inside the Connection method (in Display_Table.java)	change the database username and password (Line 47)
2. Change the .txt file path name in jButton2ActionPerformed method (Line 281)

After completing all the above steps now you will be able to run the project by clicking on Run Project button.