# Sonarqube-
sudo yum install httpd 
sudo systemctl start httpd 
sudo echo '<h1>Welcome to LandmakTechnology</h1>' >> /var/www/html/index.html 
sudo echo '<h2>Java application for a fintech</h2>' >> /var/www/html/index.html 
sudo echo '<h2>Proxy to boa-appServers</h2>' >> /var/www/html/index.html 

Multi-tier application deployment:
                Frontend-tier                  Backend-Tier
               LB/webServer-Tier    appServers-Tier        db-tier
  users---------> webServer/LB ----->appServers---------->Databases

  xml (create your tags)
     <id>01245</id>

  html (use available/predefined tags)
     <h1>Welcome to LandmakTechnology</h1>
          <h2>Proxy to boa-appServers</h2>

Software testing:
  unit testing --- Maven 
  functional 
  regression 
  perfromance 
  penetration 

echo "DevOps is good"

sonarqube:
   git/GitHub  
   src Codes  -- 9,000 lines of code  
   JUnit Tests Cases 3,000 unit test cases  
   buildScript-pom.xml 
   javaProjects 

maven :
  mvn package
     validation 
     compilation 
     JUnit-Testing [runs 3000 test cases = pass]
     packaging[jav/war/ear]

sonarqube/Benchmarking:
comparing actual results against the benchnark/standards
1. How many unit test cases were runned?
   How many test cases should have being runned? 

2. Is our code readable with ease? 
    ----> code smells 

3. Is our code portable [environment independent]?
    -- if not code smells / hard coding 

4. Are the vulnerabilities in the code ?
    ---> if they are then --- 
       password -- any 4 characters 
             1234



rules:

bugs 

maven:
mvn package 
    v / c / t / p 

    jvm = 
    javac 

  yum install maven 

  Globally 
   sudo vi /etc/profile 
  specific user 
    vi .bashrc 
    vi .bash_profile 


SonarQube / SonarCloud

Hello

SonarQube Server:
  Code coverage
    % of the code  tested by unit test cases

HelloWorld.java
	    10,000lines = 10k 
       7,000 are tested = SME 
       7000/10000*100 = 70%
 SourceCode (src) :
  mvn package:

      validation / 
         plugins / Dependencies / External libraries (remoteRepo or central repo)   
      
      compilation / 
         plugins / Dependencies / External libraries (remoteRepo or central repo)  

      testing / (Quality Gate)
         plugins / Dependencies / External libraries (remoteRepo or central repo)  
         
         run Junit Test Cases  
          Failure = maven won't buid 
          Passes = maven builds 
             mvn package DSkip 
      
      packaging(jar/war/ear)  

CodeQuality:
  boa =  code --> boa-appServers   
        build (maven (testing)) 
               tests = fail 
               no packages will be created
               mvn package 
                  RUNS 600 TESTS & 600 PASSED 
                     app.war is created 
        CODE Quality (SonarQube)
          did Developers ignore any unit test cases 
            code coverage
            scan your system identify viruses and remove them 

Application code:
HelloWorld.java() {
  1,000 lines lines of code 
}	  
JUnit TEST CASES:
HelloWorldTest.java() {
  600 unit test-cases 
  code coverage = 60%  = FAIL 
   expected code coverage = atleast 80%
}

IQ:
 What significant contribution have you introduce in LT/Team? 
    6 YEARS 
      SonarQube 
      Terraform

code coverage = 7,000/10,000*100%  =  70%  :

Code Quality expectations:
• Duplicated code
• Coding standards
• Unit tests
• Complex code
• Comments
• Potential Bugs
• Architecture & Design
Functions:

  Rules/Benchmark/standards:
    code coverage --> must be atleast 80%
        1000 LINES 
         800+ UNIT TEST CASES 
    duplicate lines must be less than 5%
      Functions: 
        userMgt{
          useradd $username
          passwd $username
        }

        fileMgt{
          touch $filename 
          chmod +x $filename
        }
  import userMgt 
  import fileMgt 

 import user 

expected code coverage for best practice should be atleast 80%

Rules:
                   standards    actual    Analysis
Lines                            1,000
JUnitTestcase                      680
code coverage        85%         68%      Failed 
duplicate lines      <5%          8%      Failed 
bugs                  0           5       Failed
vulnerabilities       0           15      Failed

code analysis compares standards against actual results:


Code Review:
  Validating standards against src (actual results)

echo "This is note 10"

 sudo yum install net-tools -y 
  netstat -tulpn 
SonarQube:
 It was originally written in Java to support Java codes ONLY

Today SonarQube supports over 20 langauges.

  Code Quality Reports  = 
    databases  = 
      volume / hard disk / hard drive (25GB)  
        Required 40GB 

  Easily readable

SonarQube:

  1. sonarqube Scanner: 

  2. sonarqube server :
       Compute engine 
       database 
       search engine - elasticsearch
       web-server

 Hello, My name is Simon, with ID:001457, . 
 
   USES ROWS AND columns  
  Excel / Word / Access
  SN    NAME      ID 
  1.    SIMON     001
  2.    Grace     002
  3.    Elvis     003
  4.    Olu       004 
  5.    Terese    005 
boa--- customer account details
  cID     cNAME     A/C bal 
  014      Paul     2,000 
  088      Israel   6,000
Structured data :
Cid Name  a/c no  a/c balance
14014 Paul  1245  2,000
15015 Grace 1255  5,000
16016 Erica 1266  7,000

unStructured data:
  JSON format:
  {
    id: 1245
    name: 'James' 
  }
 {
    SN: 6644
    name: 'Olu'
  }

Databases:
  To store Code Quality Reports 

Structured data :
RDS - Relational databases or SQL:
  SQL = Structured qwery language 
Data is written in tables format (rows and columns)
  SQL is a langague use to qwery  RDS.   :
    Oracle
    mySQL  - OS
    PostgreSql  - OS
    MSSQL (MicrosoftSQL)
    DB2
    Sybase
    MySQL, Oracle, Microsoft SQL Server, PostgreSQL
  =========
   USES ROWS AND columns  
  Excel / Word / Access
  SN    NAME      ID 
  1.    SIMON     001
  2.    Grace     002
  3.    Elvis     003
  4.    Olu       004 
  5.    Terese    005 

  SN  NAME  ID
1 BODE  LT01
2 MERCY LT02
3 PAUL  LT03


Un Structured data  :
 ['Jose 001', '4 Beatrice', 'Mercy 005'] 

noSql or nonRDS:
Data is written in Json format.
  {
    name: "simon"
    id: "MLT0012547"
    SN: "01"
  }
Examples:
    MongoDB
    Cassandra
    CouchDB, 
    CouchBase, 
    HBase, 
    Redis, 
    Riak, 
    Neo4J are the popular NoSQL databases.

connectDatabase.java() {

} 

getConnectDatabase.java(){
  if else 

  /* 

  */
 try 
 catch 
 finally 

}

Software Engineers / Developers write codes.

Who performs code review in your projects?
  Sr. Software Engineers   

SonarQube has:
 
 Free version  :
  Java,  = 30,000 lines 
  JavaScript,
  C#, 
  TypeScript,
  Kotlin,
  Ruby, Go, Scala, Flex, Python, PHP, HTML, CSS, XML and 
  VB.NET

  Java, C#, JavaScript, TypeScript, 
  CloudFormation, Terraform, Kotlin, Ruby,
  Go, Scala, Flex, Python,
  PHP, HTML, CSS, XML and VB.NET
 Installation:
  https://docs.sonarqube.org/latest/requirements/requirements/
  https://www.sonarqube.org/downloads/

https://github.com/LandmakTechnology/package-management/tree/master/soarQube-Installation
 
