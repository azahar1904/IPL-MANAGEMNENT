







CONTENTS:
CHAPTER 1: INTRODUCTION
1.1 PROJECT BACKGROUND
1.2 DESCRIPTION OF THE PROJECT
CHAPTER 2: ER DIAGRAM
2.1 ER DIAGRAM CREATION
2.2 DESCRIPTION OF ER DIAGRAM
2.3 CONVERSION OF ER DIAGRAM INTO TABLES
CHAPTER 3: TABLES
3.1 DESCRIPTION OF TABLES
3.2 NORMALISATION OF TABLES
CHAPTER 4: SQL QUERIES
4.1  CREATION OF TABLES
4.2 SQL QUERIES
4.3 CREATION OF VIEWS
CHAPTER 5: CONCLUSION

CHAPTER-1
1.1 PROJECT BACKGROUND
The IPL (Indian Premier League) Management System is designed to facilitate the management and analysis of various aspects related to the IPL cricket tournament. The IPL is a professional Twenty20 cricket league in India, contested annually by franchise teams representing different cities. The league has gained immense popularity globally, attracting top cricketing talent from around the world and generating significant interest among fans and stakeholders.
OBJECTIVE:
The IPL Management System aims to provide a comprehensive database solution for managing various aspects of the Indian Premier League (IPL). It includes functionality for managing teams, player statistics, match results, and generating insights through queries and views.
1.2 DESCRIPTION OF THE PROJECT
The project involves the development of a database schema and associated SQL queries to manage and analyze data related to teams, players, matches, and standings within the IPL. Below are the key components of the project:
Database Creation: 
The project starts with creating a database named IPL using SQL. Within this database, tables are created to store information about teams, players, and match points.
Table Structure:
TEAM_TABLE: Stores information about IPL teams, including their names and owners.
POINT_TABLE: Keeps track of each team's performance in terms of matches played, matches won, matches lost, net run rate (NRR), and total points.
Tables for individual teams (RCB, CSK, MI, etc.): Store player-specific data such as player name, jersey number, runs scored, wickets taken, player role, and team affiliation.
Data Population: The tables are populated with sample data representing players' performance and team standings.
Data Analysis Queries:
Queries are executed to analyze team standings based on points and net run rate.
Queries retrieve top performers in terms of runs scored (Orange Cap) and wickets taken (Purple Cap).
A view is created to list top all-rounders based on both runs scored and wickets taken.
Another view generates fixture information for qualifier and eliminator matches based on team standings.
A view is created to display the current team standings with position, team name, points, and net run rate.
Data Retrieval: 
Various SQL queries are executed to retrieve and display information from the database, including team standings, player performance, and upcoming match fixtures.
View Creation: 
Views are created to simplify access to frequently needed information, such as top performers and upcoming match fixtures.
Data Management: 
The project includes truncating and updating tables as needed to reflect changes in team standings and player performance.
Data Presentation: 
The results of SQL queries are presented in tabular format to facilitate readability and analysis.




































































CHAPTER 2
2.1 ER DIAGRAM


FIGURE 1: ER DIAGRAM

2.2 DESCRIPTION OF ER DIAGRAMS
TEAM_TABLE
Attributes:
TEAM_NAME (Primary Key): Represents the name of the team participating in the IPL.
OWNER_NAME: Stores the name of the owner(s) of the team.
Relationships:
This table serves as the primary entity storing information about IPL teams.


POINT_TABLE:
Attributes:
TEAM_NAME (Primary Key, Foreign Key): Links to the TEAM_NAME attribute in the TEAM_TABLE.
MATCHES_PLAYED: Indicates the total number of matches played by the team.
MATCHES_WON: Stores the count of matches won by the team.
MATCHES_LOST: Represents the count of matches lost by the team.
NRR (Net Run Rate): Measures the team's performance based on run rate.
POINTS: Stores the total points earned by the team.
Relationships:
The TEAM_NAME attribute serves as a foreign key referencing the TEAM_TABLE, establishing a one-to-one relationship between teams and their performance metrics.
Individual Team Tables (RCB, CSK, DC, MI, SRH, RR, KKR, LSG, GT, PBKS):
Attributes:
PLAYER_NAME: Holds the name of the player.
JERSEY_NO (Primary Key):  Represents the unique jersey number assigned to each player.
RUNS: Indicates the total runs scored by the player.
WICKETS: Stores the total number of wickets taken by the player.
PLAYER_ROLE: Describes the role or playing position of the player.
TEAM_NAME (Foreign Key): Links to the TEAM_NAME attribute in the TEAM_TABLE, indicating the team the player belongs to.
Relationships:
Each team table has a foreign key referencing the TEAM_TABLE, establishing a one-to-many relationship between teams and their respective players.
2.3 CONVERSION OF ER DIAGRAMS INTO TABLES:-
TEAM TABLE:-


POINT TABLE:-


RCB:-


CSK:-


MI:-


KKR:-


RR:-


LSG:-


PBKS:-


DC:-


GT:-


SRH:-



CHAPTER-3
3.1 DESCRIPTION OF TABLE

TEAM_TABLE:
Columns:
TEAM_NAME (Primary Key): Stores the name of the IPL team.
OWNER_NAME: Stores the name of the team owner.
Description: This table maintains information about IPL teams, including their names and respective owners. The TEAM_NAME column serves as the primary key to uniquely identify each team.

POINT_TABLE:
Columns:
TEAM_NAME (Primary Key, Foreign Key): References TEAM_TABLE.
MATCHES_PLAYED: Number of matches played by the team.
MATCHES_WON: Number of matches won by the team.
MATCHES_LOST: Number of matches lost by the team.
NRR: Net Run Rate of the team.
POINTS: Total points earned by the team.
Description: This table maintains the performance statistics of IPL teams, including the number of matches played, won, lost, net run rate, and total points. The TEAM_NAME column serves as both the primary key and foreign key, referencing the TEAM_TABLE.

INDIVIDUAL TEAM TABLES (RCB, CSK, DC, MI, SRH, RR, KKR, LSG, GT, PBKS):
Columns:
PLAYER_NAME: Name of the player.
JERSEY_NO (Primary Key): Jersey number of the player.
RUNS: Total runs scored by the player.
WICKETS: Total wickets taken by the player.
PLAYER_ROLE: Role of the player in the team.
TEAM_NAME (Foreign Key): References TEAM_TABLE.
Description: Each of these tables represents an IPL team and stores detailed information about the players belonging to that team. The tables include columns for player name, jersey number, runs scored, wickets taken, player role, and team affiliation. The TEAM_NAME column in each team table serves as a foreign key referencing the TEAM_TABLE.

3.2 NORMALISATION OF TABLES 

click here to view the tables in excel sheet




CHAPTER-4
4.1 CREATION OF TABLES:-

--CREATING DATABASE
CREATE DATABASE IPL;
USE IPL;

--CREATING TEAM_TABLE
CREATE TABLE IF NOT EXISTS TEAM_TABLE (
    TEAM_NAME VARCHAR(20) PRIMARY KEY,
    OWNER_NAME VARCHAR(20)
);

--CREATING POINT_TABLE
CREATE TABLE IF NOT EXISTS POINT_TABLE (
    TEAM_NAME VARCHAR(20),
    MATCHES_PLAYED INT,
    MATCHES_WON INT,
    MATCHES_LOST INT,
    NRR DECIMAL(10,2),
    POINTS INT,
    PRIMARY KEY (TEAM_NAME),
    FOREIGN KEY (TEAM_NAME) REFERENCES TEAM_TABLE(TEAM_NAME)
);

--CREATING RCB
CREATE TABLE IF NOT EXISTS RCB (
    PLAYER_NAME VARCHAR(20),
    JERSEY_NO INT PRIMARY KEY,
    RUNS INT,
    WICKETS INT,
    PLAYER_ROLE VARCHAR(20),
    TEAM_NAME VARCHAR(20),
    FOREIGN KEY (TEAM_NAME) REFERENCES TEAM_TABLE(TEAM_NAME)
);

--CREATING CSK
CREATE TABLE IF NOT EXISTS CSK (
    PLAYER_NAME VARCHAR(20),
    JERSEY_NO INT PRIMARY KEY,
    RUNS INT,
    WICKETS INT,
    PLAYER_ROLE VARCHAR(20),
    TEAM_NAME VARCHAR(20),
    FOREIGN KEY (TEAM_NAME) REFERENCES TEAM_TABLE(TEAM_NAME)
);

--CREATING DC
CREATE TABLE IF NOT EXISTS DC (
    PLAYER_NAME VARCHAR(20),
    JERSEY_NO INT PRIMARY KEY,
    RUNS INT,
    WICKETS INT,
    PLAYER_ROLE VARCHAR(20),
    TEAM_NAME VARCHAR(20),
    FOREIGN KEY (TEAM_NAME) REFERENCES TEAM_TABLE(TEAM_NAME)
);

--CREATING MI
CREATE TABLE IF NOT EXISTS MI (
    PLAYER_NAME VARCHAR(20),
    JERSEY_NO INT PRIMARY KEY,
    RUNS INT,
    WICKETS INT,
    PLAYER_ROLE VARCHAR(20),
    TEAM_NAME VARCHAR(20),
    FOREIGN KEY (TEAM_NAME) REFERENCES TEAM_TABLE(TEAM_NAME)
);
--CREATING SRH
CREATE TABLE IF NOT EXISTS SRH (
    PLAYER_NAME VARCHAR(20),
    JERSEY_NO INT PRIMARY KEY,
    RUNS INT,
    WICKETS INT,
    PLAYER_ROLE VARCHAR(20),
    TEAM_NAME VARCHAR(20),
    FOREIGN KEY (TEAM_NAME) REFERENCES TEAM_TABLE(TEAM_NAME)
);

--CREATING RR
CREATE TABLE IF NOT EXISTS RR (
    PLAYER_NAME VARCHAR(20),
    JERSEY_NO INT PRIMARY KEY,
    RUNS INT,
    WICKETS INT,
    PLAYER_ROLE VARCHAR(20),
    TEAM_NAME VARCHAR(20),
    FOREIGN KEY (TEAM_NAME) REFERENCES TEAM_TABLE(TEAM_NAME)
);

--CREATING KKR
CREATE TABLE IF NOT EXISTS KKR (
    PLAYER_NAME VARCHAR(20),
    JERSEY_NO INT PRIMARY KEY,
    RUNS INT,
    WICKETS INT,
    PLAYER_ROLE VARCHAR(20),
    TEAM_NAME VARCHAR(20),
    FOREIGN KEY (TEAM_NAME) REFERENCES TEAM_TABLE(TEAM_NAME)
);

--CREATING LSG
CREATE TABLE IF NOT EXISTS LSG (
    PLAYER_NAME VARCHAR(20),
    JERSEY_NO INT PRIMARY KEY,
    RUNS INT,
    WICKETS INT,
    PLAYER_ROLE VARCHAR(20),
    TEAM_NAME VARCHAR(20),
    FOREIGN KEY (TEAM_NAME) REFERENCES TEAM_TABLE(TEAM_NAME)
);

--CREATING GT
CREATE TABLE IF NOT EXISTS GT (
    PLAYER_NAME VARCHAR(20),
    JERSEY_NO INT PRIMARY KEY,
    RUNS INT,
    WICKETS INT,
    PLAYER_ROLE VARCHAR(20),
    TEAM_NAME VARCHAR(20),
    FOREIGN KEY (TEAM_NAME) REFERENCES TEAM_TABLE(TEAM_NAME)
);

--CREATING PBKS
CREATE TABLE IF NOT EXISTS PBKS (
    PLAYER_NAME VARCHAR(20),
    JERSEY_NO INT PRIMARY KEY,
    RUNS INT,
    WICKETS INT,
    PLAYER_ROLE VARCHAR(20),
    TEAM_NAME VARCHAR(20),
    FOREIGN KEY (TEAM_NAME) REFERENCES TEAM_TABLE(TEAM_NAME)
);

4.2 SQL QUERIES:- 

--INSERTING VALUES INTO TEAM_TABLE
insert into TEAM_TABLE values ('RCB','UNITED SPIRITS');
insert into TEAM_TABLE values ('CSK','INDIA CEMENTS');
insert into TEAM_TABLE values ('GT','CVC CAPITAL');
insert into TEAM_TABLE values ('LSG','RP SANJEEV GRP');
insert into TEAM_TABLE values ('MI','RELIANCE');
insert into TEAM_TABLE values ('RR','BLEAHEIM CHALCOT');
insert into TEAM_TABLE values ('KKR','RED CHILLIES');
insert into TEAM_TABLE values ('SRH','SUN TV');
insert into TEAM_TABLE values ('PBKS','PREITY ZINTA');
insert into TEAM_TABLE values ('DC','GMR GROUP');
select * from TEAM_TABLE;

--INSERTING VALUES INTO RCB TABLE
INSERT INTO RCB VALUES 
('VIRAT KOHLI',18,361,0,'RIGHT HAND BATSMAN','RCB'), 
('FAF DUPLESIS',13,232,0,'RIGHT HAND BATSMAN','RCB'), 
('RAJAT PATIDAR',97,109,0,'RIGHT HAND BATSMAN','RCB'), 
('ANUJ RAWAT',55,98,0,'WICKET KEEPER BATSMAN','RCB'), 
('DINESH KARTHIK',19,226,0,'WICKET KEEPER BATSMAN','RCB'), 
('GLENN MAXWELL',32,32,4,'RIGHT HAND BATSMAN, RIGHT OFF-SPIN','RCB'), 
('MAHIPAL LOMROR',6,69,0,'LEFT HAND BATSMAN, LEFT HAND OFF-SPIN','RCB'), 
('CAMERON GREEN',42,68,2,'RIGHT HAND BATSMAN, RIGHT ARM MEDIUM-PACE BOWLER','RCB'), 
('MD. SIRAJ',73,12,4,'RIGHT ARM-FAST BOWLER','RCB'), 
('YASH DAYAL',133,0,5,'LEFT ARM-MEDIUM FAST BOWLER','RCB'), 
('REECE TOPLEY',23,3,4,'LEFT ARM-FAST BOWLER','RCB'
);

--INSERTING VALUES INTO CSK TABLE
INSERT INTO CSK VALUES 
('MS DHONI',7,87,0,'WICKET KEEPER BATSMAN','CSK'), 
('RUTURAJ GAIKWAD',31,241,0,'RIGHT HAND BATSMAN','CSK'), 
('AJINKYA RAHANE',21,160,0,'RIGHT HAND BATSMAN','CSK'), 
('SAMEER RIZVI',1,15,0,'RIGHT HAND BATSMAN','CSK'), 
('RAVINDRA JADEJA',8,141,4,'LEFT HAND BATSMAN, LEFT OFF_SPIN','CSK'), 
('SHIVAN DUBE',25,245,0,'LEFT HAND BATSMAN, RIGHT ARM MEDIUM FAST','CSK'), 
('DEEPAK CHAHAR', 91, 0, 4, 'RIGHT ARM MEDIUM FAST', 'CSK'), 
('MATEESHA PATHIRANA',81,0,9,'RIGHT ARM FAST BOWLER','CSK'), 
('MUSTAFIZUR RAHMAN',90,0,11,'LEFT ARM-FAST BOWLER','CSK'), 
('TUSHAR DESHPANDE',24,0,6,'RIGHT ARM-MEDIUM FAST BOWLER','CSK'), 
('SHARDUL THAKUR',10,0,0,'RIGHT ARM MEDIUM-FAST BOWLER','CSK'
);

--INSERTING VALUES INTO SRH TABLE
INSERT INTO SRH VALUES 
('TRAVIS HEAD', 12, 235, 0, 'LEFT HAND BATSMAN', 'SRH'), 
('HEINRICH KLASEEN', 45, 253, 0, 'WICKETKEEPER BATSMAN', 'SRH'), 
('ABHISEKH SHARMA', 4, 211, 0, 'LEFT HAND BATSMAN, LEFT-ARM ORTHODOX SPINNER', 'SRH'), 
('RAHUL TRIPATHI', 52, 31, 0, 'RIGHT HAND BATSMAN', 'SRH'), 
('MAYANK AGARWAL', 16, 59, 0, 'RIGHT HAND BATSMAN', 'SRH'), 
('AIDEN MARKARAM', 7, 159, 0, 'RIGHT HAND BATSMAN', 'SRH'), 
('MARCO JANSEN', 23, 1, 0, 'LEFT HAND BATSMAN, LEFT ARM FAST BOWLER', 'SRH'), 
('SHABAZ AHMED',21,70,3,'LEFT HAND BATSMAN, LEFT ARM OFF SPIN BOWLER','SRH'), 
('PAT CUMMINS',30,5,9,'RIGHT HANDED BATSMAN, RIGHT ARM-FAST BOWLER','SRH'), 
('BHUVANESHWAR KUMAR',15,6,3,'RIGHT ARM-MEDIUM FAST BOWLER','SRH'), 
('NATRAJAN',44,0,6,'LEFT ARM MEDIUM-FAST BOWLER','SRH'
);

--INSERTING VALUES INTO DC TABLE
INSERT INTO DC VALUES 
('RISHABH PANT', 17, 210, 0, 'WICKETKEEPER BATSMAN', 'DC'), 
('DAVID WARNER', 31, 166, 0, 'LEFT HAND BATSMAN', 'DC'), 
('PRITHVI SHAW', 100, 158, 0, 'RIGHT HAND BATSMAN', 'DC'), 
('AXAR PATEL', 20, 51, 5, 'LEFT HAND BATSMAN, LEFT ARM OFF SPIN', 'DC'), 
('KULDEEP YADAV', 23, 1, 6, 'LEFT ARM ORTHODOX SPIN', 'DC'), 
('ANRICH NORTJE', 19, 4, 6, 'RIGHT ARM MEDIUM FAST BOWLER', 'DC'),
('SHAI HOPE', 4, 63, 0, 'RIGHT HAND BATSMAN', 'DC'), 
('MITCHELL MARSH', 8, 61, 1, 'RIGHT HAND BATSMAN, RIGHT ARM MEDIUM-FAST BOWLER', 'DC'), 
('MUKESH KUMAR',49,0,8,'RIGHT ARM MEDIUM-FAST BOWLER','DC'),
('ISHANT SHARMA',39,1,6,'RIGHT ARM FAST BOWLER','DC'), 
('KHALEEL AHMED',71,0,10,'LEFT ARM MEDIUM-FAST BOWLER','DC'
);

--INSERTING VALUES INTO GT TABLE
INSERT INTO GT VALUES 
('SHUBMAN GILL', 77, 263, 0, 'RIGHT HAND BATSMAN', 'GT'), 
('DAVID MILLER', 10, 79, 0, 'LEFT HAND BATSMAN', 'GT'), 
('WRIDDHIMAN SAHA', 6, 78, 0, 'WICKETKEEPER BATSMAN', 'GT'),
('KANE WILLIAMSON', 22, 27, 0, 'RIGHT HAND BATSMAN', 'GT'), 
('VIJAY SHANKAR', 59, 73, 0, 'RIGHT HAND BATTER', 'GT'), 
('RASHID KHAN', 49, 60, 7, 'LFET ARM LEG SPIN BOWLER', 'GT'),
('SHAHRUKH KHAN', 88, 14, 0, 'RIGHT HAND BATSMAN', 'GT'), 
('ABHINAV MANOHAR', 26, 9, 0, 'RIGHT HAND BATSMAN', 'GT'),
('SAI SUDARSHAN',23,238,0,'RIGHT HAND BATSMAN','GT'), 
('MOHIT SHARMA',27,2,8,'RIGHT ARM MEDIUM-FAST BOWLER','GT'), 
('NOOR AHMED',15,2,3,'LEFT ARM LEG SPIN BOWLER','GT'
);

--INSERTING VALUES INTO KKR TABLE
INSERT INTO KKR VALUES 
('SHREYAS IYER', 18, 140, 0, 'RIGHT HAND BATSMAN', 'KKR'), 
('NITISH RANA', 27, 9, 0, 'LEFT HAND BATSMAN', 'KKR'),
('RINKU SINGH', 3, 83, 0, 'LEFT HAND BATSMAN', 'KKR'),
('VENKATESH IYER', 41, 73, 0, 'LEFT HAND BATSMAN, RIGHT ARM MEDIUM FAST BOWLER', 'KKR'), 
('SUNIL NARINE', 74, 276, 7, 'RIGHT ARM OFF SPIN', 'KKR'),
('ANDRE RUSSELL', 12, 128, 6, 'RIGHT HAND BATSMAN, RIGHT ARM MEDIUM FAST', 'KKR'),
('SUYASH SHARMA', 23, 0, 0, 'RIGHT ARM LEG SPIN', 'KKR'),
('HARSHIT RANA', 8, 0, 7, 'RIGHT ARM MEDIUM FAST BOWLER', 'KKR'),
('VARUN CHAKRAVARTHY',29,0,7,'RIGHT ARM OFF SPIN','KKR'), 
('MITCHEL STARC',56,7,5,'LEFT ARM FAST BOWLER','GT'), 
('PHIL SALT',61,201,0,'RIGHT HAND BATSMAN','KKR'
);

--INSERTING VALUES INTO LSG TABLE;
INSERT INTO LSG VALUES 
('KL RAHUL', 1, 286, 0, 'WICKETKEEPER BATSMAN', 'LSG'),
('QUINTON DE KOCK', 20, 228, 0, 'WICKETKEEPER BATSMAN', 'LSG'),
('NICHOLAS POORAN', 29, 246, 0, 'WICKETKEEPER BATSMAN', 'LSG'),
('DEEPAK HOODA', 5, 44, 0, 'RIGHT HAND BATSMAN', 'LSG'),
('KRUNAL PANDYA', 24, 58, 5, 'LEFT HAND BATSMAN, LEFT ARM OFF SPIN', 'LSG'),
('MARCUS STOINIS', 17, 130, 2, 'RIGHT HAND BATSMAN, RIGHT ARM MEDIUM-FAST BOWLER', 'LSG'),
('RAVI BISHNOI', 3, 0, 5, 'RIGHT ARM LEG SPIN', 'LSG'),
('AYUSH BADONI', 50, 113, 0, 'RIGHT HAND BATSMAN', 'LSG'),
('NAVEEN UL HAQ',78,0,6,'RIGHT ARM FAST BOWLER','LSG'),
('DEVDUTT PADIKKAL',37,25,0,'LEFT HAND BATSMAN','LSG'),
('MOHSIN KHAN',47,2,6,'LEFT ARM FAST BOWLER','LSG'
);

--INSERTING VALUES INTO MI TABLE
INSERT INTO MI VALUES 
('ROHIT SHARMA', 45, 297, 0, 'RIGHT HAND BATSMAN', 'MI'),
('ISHAN KISHAN', 32, 192, 0, 'WICKETKEEPER BATSMAN', 'MI'),
('SURYAKUMAR YADAV', 77, 130, 0, 'RIGHT HAND BATSMAN', 'MI'),
('TIM DAVID', 1, 142, 0, 'RIGHT HAND BATSMAN', 'MI'),
('TILAK VARMA', 23, 208, 0, 'LEFT HAND BATSMAN', 'MI'),
('HARDIK PANDYA', 33, 141, 4, 'RIGHT HAND BATSMAN, RIGHT HAND MEDIUM FAST', 'MI'),
('JASPRIT BUMRAH', 93, 9, 13, 'RIGHT ARM FAST BOWLER', 'MI'),
('GERALD CORTZEE', 25,5, 12, 'RIGHT ARM FAST BOWLER', 'MI'), 
('MD. NABI',17,4,0,'RIGHT HAND BATSMAN, RIGHT ARM OFF SPIN','MI'),
('PIYUSH CHAWLA',30,3,2,'RIGHT ARM LEG SPIN BOWLER','MI'), 
('MOHSIN KHAN',75,4,5,'RIGHT ARM MEDIUM-FAST BOWLER','MI'
);


--INSERTING VALUES INTO PBKS TABLE
INSERT INTO PBKS VALUES 
('SHIKHAR DHAWAN', 42, 152, 0, 'LEFT HAND BATSMAN', 'PBKS'),
('JONNY BAIRSTOW', 51, 96, 0, 'WICKETKEEPER BATTER', 'PBKS'),
('JITESH SHARMA', 12, 115, 0, 'WICKETKEEPER BATSMAN', 'PBKS'),
('SAM CURRAN', 58, 132, 10, 'LEFT HAND BATSMAN, LEFT ARM FAST BOWLER', 'PBKS'),
('LIAM LIVINGSTONE', 4, 105, 1, 'RIGHT HAND BATSMAN, RIGHT ARM OFF SPIN', 'PBKS'),
('ASHUTOSH SHARMA', 22, 156, 0, 'RIGHT HAND BATSMAN', 'PBKS'),
('SHASHANK SINGH', 27, 187, 0, 'RIGHT HAND BATSMAN', 'PBKS'),
('PRABHSIMRAN SINGH', 53,119, 0, 'RIGHT HAND BATSMAN', 'PBKS'),
('KASIGO RABADA',25,8,10,'RIGHT ARM FAST BOWLER','PBKS'),
('ARSHDEEP SINGH',2,0,9,'LEFT ARM FAST BOWLER','PBKS'),
('MOHSIN KHAN',75,4,5,'RIGHT ARM MEDIUM-FAST BOWLER','PBKS');

--INSERTING VALUES INTO RR TABLE
INSERT INTO RR VALUES ('SANJU SAMSON', 7, 276, 0, 'WICKETKEEPER BATSMAN', 'RR'),('JOS BUTTLER', 63, 250, 0, 'RIGHT HAND BATSMAN', 'RR'),('SHIMRON HETMYER', 14, 70, 0, 'LEFT HAND BATSMAN', 'RR'),('RIYAN PARAG', 5, 318, 0, 'RIGHT HAND BATSMAN', 'RR'),('YASHASVI JAISWAL', 121, 0, 0, 'LEFT HAND BATSMAN', 'RR'),('RAVICHANDRAN ASWIN', 99, 53, 1, 'RIGHT HAND BATSMAN, RIGHT ARM OFF SPIN', 'RR'),('ROVMAN POWELL', 22, 37, 0, 'RIGHT HAND BATSMAN', 'RR'),('YUZIVENDRA CHAHAL', 3,0, 12, 'RIGHT ARM LEG SPIN', 'RR'), ('TRENT BOULT',18,0,7,'LEFT ARM FAST BOWLER','RR'), ('AVESH KHAN',6,0,7,'RIGHT ARM FAST BOWLER','RR'), ('DHRUV JUREL',21,50,0,'RIGHT HAND BATSMAN','RR');

select * from DC;
select * from RCB;
select * from CSK;
select * from MI;
select * from GT;
select * from LSG;
select * from RR;
select * from KKR;
select * from PBKS;
select * from SRH;

--INSERTING VALUES INTO POINT_TABLE
INSERT INTO POINT_TABLE VALUES 
('RR',7,6,1,0.677,12), 
('KKR',6,4,2,1.399,8), 
('CSK',7,4,3,0.529,8),
('RCB',6,4,2,0.502,8),
('LSG',7,4,3,0.123,8),
('DC',7,3,4,-0.074,6),
('MI',7,3,4,-0.133,6),
('GT',7,3,4,-1.303,6),
('PBKS',7,2,5,-0.251,4),
('SRH',7,1,6,-1.185,2
);
SELECT * FROM POINT_TABLE
ORDER BY POINTS desc,NRR desc;
SELECT * FROM RCB ORDER BY RUNS DESC LIMIT 5;

4.3 CREATION OF VIEWS:- 

--CREATION OF VIEW FOR ORANGE CAP
CREATE VIEW ORANGE_CAP AS
SELECT PLAYER_NAME, JERSEY_NO, RUNS, TEAM_NAME
FROM (
    SELECT PLAYER_NAME, JERSEY_NO, RUNS, TEAM_NAME
    FROM RCB
    UNION ALL
    SELECT PLAYER_NAME, JERSEY_NO, RUNS, TEAM_NAME
    FROM CSK
    UNION ALL
    SELECT PLAYER_NAME, JERSEY_NO, RUNS, TEAM_NAME
    FROM DC
    UNION ALL
    SELECT PLAYER_NAME, JERSEY_NO, RUNS, TEAM_NAME
    FROM MI
    UNION ALL
    SELECT PLAYER_NAME, JERSEY_NO, RUNS, TEAM_NAME
    FROM GT
    UNION ALL
    SELECT PLAYER_NAME, JERSEY_NO, RUNS, TEAM_NAME
    FROM LSG
    UNION ALL
    SELECT PLAYER_NAME, JERSEY_NO, RUNS, TEAM_NAME
    FROM RR
    UNION ALL
    SELECT PLAYER_NAME, JERSEY_NO, RUNS, TEAM_NAME
    FROM KKR
    UNION ALL
    SELECT PLAYER_NAME, JERSEY_NO, RUNS, TEAM_NAME
    FROM PBKS
    UNION ALL
    SELECT PLAYER_NAME, JERSEY_NO, RUNS, TEAM_NAME
    FROM SRH
) AS ALL_PLAYERS
ORDER BY RUNS DESC
LIMIT 10;

--CREATION OF VIEW FOR PURPLE CAP
CREATE VIEW PURPLE_CAP AS
SELECT PLAYER_NAME, JERSEY_NO, WICKETS, TEAM_NAME
FROM (
    SELECT PLAYER_NAME, JERSEY_NO, WICKETS, TEAM_NAME
    FROM RCB
    UNION ALL
    SELECT PLAYER_NAME, JERSEY_NO, WICKETS, TEAM_NAME
    FROM CSK
    UNION ALL
    SELECT PLAYER_NAME, JERSEY_NO, WICKETS, TEAM_NAME
    FROM DC
    UNION ALL
    SELECT PLAYER_NAME, JERSEY_NO, WICKETS, TEAM_NAME
    FROM MI
    UNION ALL
    SELECT PLAYER_NAME, JERSEY_NO, WICKETS, TEAM_NAME
    FROM GT
    UNION ALL
    SELECT PLAYER_NAME, JERSEY_NO, WICKETS, TEAM_NAME
    FROM LSG
    UNION ALL
    SELECT PLAYER_NAME, JERSEY_NO, WICKETS, TEAM_NAME
    FROM RR
    UNION ALL
    SELECT PLAYER_NAME, JERSEY_NO, WICKETS, TEAM_NAME
    FROM KKR
    UNION ALL
    SELECT PLAYER_NAME, JERSEY_NO, WICKETS, TEAM_NAME
    FROM PBKS
    UNION ALL
    SELECT PLAYER_NAME, JERSEY_NO, WICKETS, TEAM_NAME
    FROM SRH
) AS ALL_PLAYERS
ORDER BY WICKETS DESC
LIMIT 10;
--CREATION OF VIEW FOR BEST ALLROUNDERS
CREATE VIEW ALLROUNDER_LIST AS
SELECT PLAYER_NAME, JERSEY_NO, TEAM_NAME, RUNS, WICKETS
FROM (
    SELECT PLAYER_NAME, JERSEY_NO, TEAM_NAME, RUNS, WICKETS
    FROM RCB
    UNION ALL
    SELECT PLAYER_NAME, JERSEY_NO, TEAM_NAME, RUNS, WICKETS
    FROM CSK
    UNION ALL
    SELECT PLAYER_NAME, JERSEY_NO, TEAM_NAME, RUNS, WICKETS
    FROM DC
    UNION ALL
    SELECT PLAYER_NAME, JERSEY_NO, TEAM_NAME, RUNS, WICKETS
    FROM MI
    UNION ALL
    SELECT PLAYER_NAME, JERSEY_NO, TEAM_NAME, RUNS, WICKETS
    FROM GT
    UNION ALL
    SELECT PLAYER_NAME, JERSEY_NO, TEAM_NAME, RUNS, WICKETS
    FROM LSG
    UNION ALL
    SELECT PLAYER_NAME, JERSEY_NO, TEAM_NAME, RUNS, WICKETS
    FROM RR
    UNION ALL
    SELECT PLAYER_NAME, JERSEY_NO, TEAM_NAME, RUNS, WICKETS
    FROM KKR
    UNION ALL
    SELECT PLAYER_NAME, JERSEY_NO, TEAM_NAME, RUNS, WICKETS
    FROM PBKS
    UNION ALL
    SELECT PLAYER_NAME, JERSEY_NO, TEAM_NAME, RUNS, WICKETS
    FROM SRH
) AS ALL_PLAYERS
WHERE RUNS >= 50 AND WICKETS >= 1
ORDER BY (RUNS + (WICKETS * 10)) DESC
LIMIT 10;

--CREATION OF VIEW FOR PLAYOFFS
CREATE VIEW QUALIFIER_FIXTURES AS
SELECT CONCAT('QUALIFIER ', q1.team1, ' VS ', q1.team2) AS FIXTURE
FROM (
    SELECT pt1.TEAM_NAME AS team1, pt2.TEAM_NAME AS team2
    FROM POINT_TABLE pt1, POINT_TABLE pt2
    WHERE pt1.TEAM_NAME < pt2.TEAM_NAME
    ORDER BY pt1.POINTS DESC, pt2.POINTS DESC
    LIMIT 1
) q1
UNION ALL
SELECT CONCAT('ELIMINATOR 1 ', q2.team1, ' VS ', q2.team2) AS FIXTURE
FROM (
    SELECT pt1.TEAM_NAME AS team1, pt2.TEAM_NAME AS team2
    FROM POINT_TABLE pt1, POINT_TABLE pt2
    WHERE pt1.TEAM_NAME < pt2.TEAM_NAME
    ORDER BY pt1.POINTS DESC, pt2.POINTS DESC
    LIMIT 1, 1
) q2;

--CREATION OF VIEW FOR TEAMS STANDING
CREATE VIEW TEAM_STANDINGS AS
SELECT ROW_NUMBER() OVER (ORDER BY POINTS DESC, NRR DESC) AS POSITION, TEAM_NAME, POINTS, NRR
FROM POINT_TABLE;
DROP VIEW IF EXISTS TEAM_STANDINGS;
SELECT * FROM ORANGE_CAP;
SELECT * FROM PURPLE_CAP;
SELECT * FROM ALLROUNDER_LIST;
SELECT * FROM QUALIFIER_FIXTURES;
SELECT * FROM TEAM_STANDINGS;









CHAPTER-5
CONCLUSION:
The IPL Management System project successfully demonstrates the implementation of a relational database model to manage IPL team and player data effectively.
The IPL database project provides a comprehensive platform for managing and analyzing cricket team data. Through this project, we have:

Established Database Structure: Designed a well-structured relational database consisting of tables for teams, player statistics, and match points.
Data Entry and Management: Populated the database with team information, player statistics, and match points using SQL queries.
Data Analysis: Conducted various analyses such as finding the top run-scorers and wicket-takers, identifying all-rounders, determining team standings, and generating fixtures for qualifiers.
Views for Easy Access: Created views like ORANGE_CAP, PURPLE_CAP, ALLROUNDER_LIST, and QUALIFIER_FIXTURES to simplify access to important information.
Team Standings: Developed a view TEAM_STANDINGS to showcase the current standings of teams based on points and net run rate.

By utilizing SQL queries and database operations, the system provides a robust platform for IPL administrators, team owners, and fans to track and analyze the performance of teams and players throughout the tournament.
This project provides valuable insights for team management, player performance evaluation, and fixture scheduling. It can be further expanded to incorporate additional features such as real-time data updates, user interfaces for data entry, and advanced analytics. Overall, the IPL database project serves as a robust platform for cricket enthusiasts, analysts, and team management alike.
