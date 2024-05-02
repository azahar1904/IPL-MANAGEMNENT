-- phpMyAdmin SQL Dump
-- version 5.2.1
-- https://www.phpmyadmin.net/
--
-- Host: 127.0.0.1
-- Generation Time: May 02, 2024 at 07:16 PM
-- Server version: 10.4.32-MariaDB
-- PHP Version: 8.2.12

SET SQL_MODE = "NO_AUTO_VALUE_ON_ZERO";
START TRANSACTION;
SET time_zone = "+00:00";


/*!40101 SET @OLD_CHARACTER_SET_CLIENT=@@CHARACTER_SET_CLIENT */;
/*!40101 SET @OLD_CHARACTER_SET_RESULTS=@@CHARACTER_SET_RESULTS */;
/*!40101 SET @OLD_COLLATION_CONNECTION=@@COLLATION_CONNECTION */;
/*!40101 SET NAMES utf8mb4 */;

--
-- Database: `ipl`
--

-- --------------------------------------------------------

--
-- Stand-in structure for view `allrounder_list`
-- (See below for the actual view)
--
CREATE TABLE `allrounder_list` (
`PLAYER_NAME` varchar(20)
,`JERSEY_NO` int(11)
,`TEAM_NAME` varchar(20)
,`RUNS` int(11)
,`WICKETS` int(11)
);

-- --------------------------------------------------------

--
-- Table structure for table `csk`
--

CREATE TABLE `csk` (
  `PLAYER_NAME` varchar(20) DEFAULT NULL,
  `JERSEY_NO` int(11) NOT NULL,
  `RUNS` int(11) DEFAULT NULL,
  `WICKETS` int(11) DEFAULT NULL,
  `PLAYER_ROLE` varchar(20) DEFAULT NULL,
  `TEAM_NAME` varchar(20) DEFAULT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci;

--
-- Dumping data for table `csk`
--

INSERT INTO `csk` (`PLAYER_NAME`, `JERSEY_NO`, `RUNS`, `WICKETS`, `PLAYER_ROLE`, `TEAM_NAME`) VALUES
('SAMEER RIZVI', 1, 15, 0, 'RIGHT HAND BATSMAN', 'CSK'),
('MS DHONI', 7, 87, 0, 'WICKET KEEPER BATSMA', 'CSK'),
('RAVINDRA JADEJA', 8, 141, 4, 'LEFT HAND BATSMAN, L', 'CSK'),
('SHARDUL THAKUR', 10, 0, 0, 'RIGHT ARM MEDIUM-FAS', 'CSK'),
('AJINKYA RAHANE', 21, 160, 0, 'RIGHT HAND BATSMAN', 'CSK'),
('TUSHAR DESHPANDE', 24, 0, 6, 'RIGHT ARM-MEDIUM FAS', 'CSK'),
('SHIVAN DUBE', 25, 245, 0, 'LEFT HAND BATSMAN, R', 'CSK'),
('RUTURAJ GAIKWAD', 31, 241, 0, 'RIGHT HAND BATSMAN', 'CSK'),
('MATEESHA PATHIRANA', 81, 0, 9, 'RIGHT ARM FAST BOWLE', 'CSK'),
('MUSTAFIZUR RAHMAN', 90, 0, 11, 'LEFT ARM-FAST BOWLER', 'CSK'),
('DEEPAK CHAHAR', 91, 0, 4, 'RIGHT ARM MEDIUM FAS', 'CSK');

-- --------------------------------------------------------

--
-- Table structure for table `dc`
--

CREATE TABLE `dc` (
  `PLAYER_NAME` varchar(20) DEFAULT NULL,
  `JERSEY_NO` int(11) NOT NULL,
  `RUNS` int(11) DEFAULT NULL,
  `WICKETS` int(11) DEFAULT NULL,
  `PLAYER_ROLE` varchar(20) DEFAULT NULL,
  `TEAM_NAME` varchar(20) DEFAULT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci;

--
-- Dumping data for table `dc`
--

INSERT INTO `dc` (`PLAYER_NAME`, `JERSEY_NO`, `RUNS`, `WICKETS`, `PLAYER_ROLE`, `TEAM_NAME`) VALUES
('SHAI HOPE', 4, 63, 0, 'RIGHT HAND BATSMAN', 'DC'),
('MITCHELL MARSH', 8, 61, 1, 'RIGHT HAND BATSMAN, ', 'DC'),
('RISHABH PANT', 17, 210, 0, 'WICKETKEEPER BATSMAN', 'DC'),
('ANRICH NORTJE', 19, 4, 6, 'RIGHT ARM MEDIUM FAS', 'DC'),
('AXAR PATEL', 20, 51, 5, 'LEFT HAND BATSMAN, L', 'DC'),
('KULDEEP YADAV', 23, 1, 6, 'LEFT ARM ORTHODOX SP', 'DC'),
('DAVID WARNER', 31, 166, 0, 'LEFT HAND BATSMAN', 'DC'),
('ISHANT SHARMA', 39, 1, 6, 'RIGHT ARM FAST BOWLE', 'DC'),
('MUKESH KUMAR', 49, 0, 8, 'RIGHT ARM MEDIUM-FAS', 'DC'),
('KHALEEL AHMED', 71, 0, 10, 'LEFT ARM MEDIUM-FAST', 'DC'),
('PRITHVI SHAW', 100, 158, 0, 'RIGHT HAND BATSMAN', 'DC');

-- --------------------------------------------------------

--
-- Table structure for table `gt`
--

CREATE TABLE `gt` (
  `PLAYER_NAME` varchar(20) DEFAULT NULL,
  `JERSEY_NO` int(11) NOT NULL,
  `RUNS` int(11) DEFAULT NULL,
  `WICKETS` int(11) DEFAULT NULL,
  `PLAYER_ROLE` varchar(20) DEFAULT NULL,
  `TEAM_NAME` varchar(20) DEFAULT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci;

--
-- Dumping data for table `gt`
--

INSERT INTO `gt` (`PLAYER_NAME`, `JERSEY_NO`, `RUNS`, `WICKETS`, `PLAYER_ROLE`, `TEAM_NAME`) VALUES
('WRIDDHIMAN SAHA', 6, 78, 0, 'WICKETKEEPER BATSMAN', 'GT'),
('DAVID MILLER', 10, 79, 0, 'LEFT HAND BATSMAN', 'GT'),
('NOOR AHMED', 15, 2, 3, 'LEFT ARM LEG SPIN BO', 'GT'),
('KANE WILLIAMSON', 22, 27, 0, 'RIGHT HAND BATSMAN', 'GT'),
('SAI SUDARSHAN', 23, 238, 0, 'RIGHT HAND BATSMAN', 'GT'),
('ABHINAV MANOHAR', 26, 9, 0, 'RIGHT HAND BATSMAN', 'GT'),
('MOHIT SHARMA', 27, 2, 8, 'RIGHT ARM MEDIUM-FAS', 'GT'),
('RASHID KHAN', 49, 60, 7, 'LFET ARM LEG SPIN BO', 'GT'),
('VIJAY SHANKAR', 59, 73, 0, 'RIGHT HAND BATTER', 'GT'),
('SHUBMAN GILL', 77, 263, 0, 'RIGHT HAND BATSMAN', 'GT'),
('SHAHRUKH KHAN', 88, 14, 0, 'RIGHT HAND BATSMAN', 'GT');

-- --------------------------------------------------------

--
-- Table structure for table `kkr`
--

CREATE TABLE `kkr` (
  `PLAYER_NAME` varchar(20) DEFAULT NULL,
  `JERSEY_NO` int(11) NOT NULL,
  `RUNS` int(11) DEFAULT NULL,
  `WICKETS` int(11) DEFAULT NULL,
  `PLAYER_ROLE` varchar(20) DEFAULT NULL,
  `TEAM_NAME` varchar(20) DEFAULT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci;

--
-- Dumping data for table `kkr`
--

INSERT INTO `kkr` (`PLAYER_NAME`, `JERSEY_NO`, `RUNS`, `WICKETS`, `PLAYER_ROLE`, `TEAM_NAME`) VALUES
('RINKU SINGH', 3, 83, 0, 'LEFT HAND BATSMAN', 'KKR'),
('HARSHIT RANA', 8, 0, 7, 'RIGHT ARM MEDIUM FAS', 'KKR'),
('ANDRE RUSSELL', 12, 128, 6, 'RIGHT HAND BATSMAN, ', 'KKR'),
('SHREYAS IYER', 18, 140, 0, 'RIGHT HAND BATSMAN', 'KKR'),
('SUYASH SHARMA', 23, 0, 0, 'RIGHT ARM LEG SPIN', 'KKR'),
('NITISH RANA', 27, 9, 0, 'LEFT HAND BATSMAN', 'KKR'),
('VARUN CHAKRAVARTHY', 29, 0, 7, 'RIGHT ARM OFF SPIN', 'KKR'),
('VENKATESH IYER', 41, 73, 0, 'LEFT HAND BATSMAN, R', 'KKR'),
('MITCHEL STARC', 56, 7, 5, 'LEFT ARM FAST BOWLER', 'GT'),
('PHIL SALT', 61, 201, 0, 'RIGHT HAND BATSMAN', 'KKR'),
('SUNIL NARINE', 74, 276, 7, 'RIGHT ARM OFF SPIN', 'KKR');

-- --------------------------------------------------------

--
-- Table structure for table `lsg`
--

CREATE TABLE `lsg` (
  `PLAYER_NAME` varchar(20) DEFAULT NULL,
  `JERSEY_NO` int(11) NOT NULL,
  `RUNS` int(11) DEFAULT NULL,
  `WICKETS` int(11) DEFAULT NULL,
  `PLAYER_ROLE` varchar(20) DEFAULT NULL,
  `TEAM_NAME` varchar(20) DEFAULT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci;

--
-- Dumping data for table `lsg`
--

INSERT INTO `lsg` (`PLAYER_NAME`, `JERSEY_NO`, `RUNS`, `WICKETS`, `PLAYER_ROLE`, `TEAM_NAME`) VALUES
('KL RAHUL', 1, 286, 0, 'WICKETKEEPER BATSMAN', 'LSG'),
('RAVI BISHNOI', 3, 0, 5, 'RIGHT ARM LEG SPIN', 'LSG'),
('DEEPAK HOODA', 5, 44, 0, 'RIGHT HAND BATSMAN', 'LSG'),
('MARCUS STOINIS', 17, 130, 2, 'RIGHT HAND BATSMAN, ', 'LSG'),
('QUINTON DE KOCK', 20, 228, 0, 'WICKETKEEPER BATSMAN', 'LSG'),
('KRUNAL PANDYA', 24, 58, 5, 'LEFT HAND BATSMAN, L', 'LSG'),
('NICHOLAS POORAN', 29, 246, 0, 'WICKETKEEPER BATSMAN', 'LSG'),
('DEVDUTT PADIKKAL', 37, 25, 0, 'LEFT HAND BATSMAN', 'LSG'),
('MOHSIN KHAN', 47, 2, 6, 'LEFT ARM FAST BOWLER', 'LSG'),
('AYUSH BADONI', 50, 113, 0, 'RIGHT HAND BATSMAN', 'LSG'),
('NAVEEN UL HAQ', 78, 0, 6, 'RIGHT ARM FAST BOWLE', 'LSG');

-- --------------------------------------------------------

--
-- Table structure for table `mi`
--

CREATE TABLE `mi` (
  `PLAYER_NAME` varchar(20) DEFAULT NULL,
  `JERSEY_NO` int(11) NOT NULL,
  `RUNS` int(11) DEFAULT NULL,
  `WICKETS` int(11) DEFAULT NULL,
  `PLAYER_ROLE` varchar(20) DEFAULT NULL,
  `TEAM_NAME` varchar(20) DEFAULT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci;

--
-- Dumping data for table `mi`
--

INSERT INTO `mi` (`PLAYER_NAME`, `JERSEY_NO`, `RUNS`, `WICKETS`, `PLAYER_ROLE`, `TEAM_NAME`) VALUES
('TIM DAVID', 1, 142, 0, 'RIGHT HAND BATSMAN', 'MI'),
('MD. NABI', 17, 4, 0, 'RIGHT HAND BATSMAN, ', 'MI'),
('TILAK VARMA', 23, 208, 0, 'LEFT HAND BATSMAN', 'MI'),
('GERALD CORTZEE', 25, 5, 12, 'RIGHT ARM FAST BOWLE', 'MI'),
('PIYUSH CHAWLA', 30, 3, 2, 'RIGHT ARM LEG SPIN B', 'MI'),
('ISHAN KISHAN', 32, 192, 0, 'WICKETKEEPER BATSMAN', 'MI'),
('HARDIK PANDYA', 33, 141, 4, 'RIGHT HAND BATSMAN, ', 'MI'),
('ROHIT SHARMA', 45, 297, 0, 'RIGHT HAND BATSMAN', 'MI'),
('MOHSIN KHAN', 75, 4, 5, 'RIGHT ARM MEDIUM-FAS', 'MI'),
('SURYAKUMAR YADAV', 77, 130, 0, 'RIGHT HAND BATSMAN', 'MI'),
('JASPRIT BUMRAH', 93, 9, 13, 'RIGHT ARM FAST BOWLE', 'MI');

-- --------------------------------------------------------

--
-- Stand-in structure for view `orange_cap`
-- (See below for the actual view)
--
CREATE TABLE `orange_cap` (
`PLAYER_NAME` varchar(20)
,`JERSEY_NO` int(11)
,`RUNS` int(11)
,`TEAM_NAME` varchar(20)
);

-- --------------------------------------------------------

--
-- Table structure for table `pbks`
--

CREATE TABLE `pbks` (
  `PLAYER_NAME` varchar(20) DEFAULT NULL,
  `JERSEY_NO` int(11) NOT NULL,
  `RUNS` int(11) DEFAULT NULL,
  `WICKETS` int(11) DEFAULT NULL,
  `PLAYER_ROLE` varchar(20) DEFAULT NULL,
  `TEAM_NAME` varchar(20) DEFAULT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci;

--
-- Dumping data for table `pbks`
--

INSERT INTO `pbks` (`PLAYER_NAME`, `JERSEY_NO`, `RUNS`, `WICKETS`, `PLAYER_ROLE`, `TEAM_NAME`) VALUES
('ARSHDEEP SINGH', 2, 0, 9, 'LEFT ARM FAST BOWLER', 'PBKS'),
('LIAM LIVINGSTONE', 4, 105, 1, 'RIGHT HAND BATSMAN, ', 'PBKS'),
('JITESH SHARMA', 12, 115, 0, 'WICKETKEEPER BATSMAN', 'PBKS'),
('ASHUTOSH SHARMA', 22, 156, 0, 'RIGHT HAND BATSMAN', 'PBKS'),
('KASIGO RABADA', 25, 8, 10, 'RIGHT ARM FAST BOWLE', 'PBKS'),
('SHASHANK SINGH', 27, 187, 0, 'RIGHT HAND BATSMAN', 'PBKS'),
('SHIKHAR DHAWAN', 42, 152, 0, 'LEFT HAND BATSMAN', 'PBKS'),
('JONNY BAIRSTOW', 51, 96, 0, 'WICKETKEEPER BATTER', 'PBKS'),
('PRABHSIMRAN SINGH', 53, 119, 0, 'RIGHT HAND BATSMAN', 'PBKS'),
('SAM CURRAN', 58, 132, 10, 'LEFT HAND BATSMAN, L', 'PBKS'),
('MOHSIN KHAN', 75, 4, 5, 'RIGHT ARM MEDIUM-FAS', 'PBKS');

-- --------------------------------------------------------

--
-- Table structure for table `point_table`
--

CREATE TABLE `point_table` (
  `TEAM_NAME` varchar(20) NOT NULL,
  `MATCHES_PLAYED` int(11) DEFAULT NULL,
  `MATCHES_WON` int(11) DEFAULT NULL,
  `MATCHES_LOST` int(11) DEFAULT NULL,
  `NRR` decimal(10,2) DEFAULT NULL,
  `POINTS` int(11) DEFAULT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci;

--
-- Dumping data for table `point_table`
--

INSERT INTO `point_table` (`TEAM_NAME`, `MATCHES_PLAYED`, `MATCHES_WON`, `MATCHES_LOST`, `NRR`, `POINTS`) VALUES
('CSK', 7, 4, 3, 0.53, 8),
('DC', 7, 3, 4, -0.07, 6),
('GT', 7, 3, 4, -1.30, 6),
('KKR', 6, 4, 2, 1.40, 8),
('LSG', 7, 4, 3, 0.12, 8),
('MI', 7, 3, 4, -0.13, 6),
('PBKS', 7, 2, 5, -0.25, 4),
('RCB', 6, 4, 2, 0.50, 8),
('RR', 7, 6, 1, 0.68, 12),
('SRH', 7, 1, 6, -1.19, 2);

-- --------------------------------------------------------

--
-- Stand-in structure for view `purple_cap`
-- (See below for the actual view)
--
CREATE TABLE `purple_cap` (
`PLAYER_NAME` varchar(20)
,`JERSEY_NO` int(11)
,`WICKETS` int(11)
,`TEAM_NAME` varchar(20)
);

-- --------------------------------------------------------

--
-- Stand-in structure for view `qualifier_fixtures`
-- (See below for the actual view)
--
CREATE TABLE `qualifier_fixtures` (
`FIXTURE` varchar(57)
);

-- --------------------------------------------------------

--
-- Table structure for table `rcb`
--

CREATE TABLE `rcb` (
  `PLAYER_NAME` varchar(20) DEFAULT NULL,
  `JERSEY_NO` int(11) NOT NULL,
  `RUNS` int(11) DEFAULT NULL,
  `WICKETS` int(11) DEFAULT NULL,
  `PLAYER_ROLE` varchar(20) DEFAULT NULL,
  `TEAM_NAME` varchar(20) DEFAULT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci;

--
-- Dumping data for table `rcb`
--

INSERT INTO `rcb` (`PLAYER_NAME`, `JERSEY_NO`, `RUNS`, `WICKETS`, `PLAYER_ROLE`, `TEAM_NAME`) VALUES
('MAHIPAL LOMROR', 6, 69, 0, 'LEFT HAND BATSMAN, L', 'RCB'),
('FAF DUPLESIS', 13, 232, 0, 'RIGHT HAND BATSMAN', 'RCB'),
('VIRAT KOHLI', 18, 361, 0, 'RIGHT HAND BATSMAN', 'RCB'),
('DINESH KARTHIK', 19, 226, 0, 'WICKET KEEPER BATSMA', 'RCB'),
('REECE TOPLEY', 23, 3, 4, 'LEFT ARM-FAST BOWLER', 'RCB'),
('GLENN MAXWELL', 32, 32, 4, 'RIGHT HAND BATSMAN, ', 'RCB'),
('CAMERON GREEN', 42, 68, 2, 'RIGHT HAND BATSMAN, ', 'RCB'),
('ANUJ RAWAT', 55, 98, 0, 'WICKET KEEPER BATSMA', 'RCB'),
('MD. SIRAJ', 73, 12, 4, 'RIGHT ARM-FAST BOWLE', 'RCB'),
('RAJAT PATIDAR', 97, 109, 0, 'RIGHT HAND BATSMAN', 'RCB'),
('YASH DAYAL', 133, 0, 5, 'LEFT ARM-MEDIUM FAST', 'RCB');

-- --------------------------------------------------------

--
-- Table structure for table `rr`
--

CREATE TABLE `rr` (
  `PLAYER_NAME` varchar(20) DEFAULT NULL,
  `JERSEY_NO` int(11) NOT NULL,
  `RUNS` int(11) DEFAULT NULL,
  `WICKETS` int(11) DEFAULT NULL,
  `PLAYER_ROLE` varchar(20) DEFAULT NULL,
  `TEAM_NAME` varchar(20) DEFAULT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci;

--
-- Dumping data for table `rr`
--

INSERT INTO `rr` (`PLAYER_NAME`, `JERSEY_NO`, `RUNS`, `WICKETS`, `PLAYER_ROLE`, `TEAM_NAME`) VALUES
('YUZIVENDRA CHAHAL', 3, 0, 12, 'RIGHT ARM LEG SPIN', 'RR'),
('RIYAN PARAG', 5, 318, 0, 'RIGHT HAND BATSMAN', 'RR'),
('AVESH KHAN', 6, 0, 7, 'RIGHT ARM FAST BOWLE', 'RR'),
('SANJU SAMSON', 7, 276, 0, 'WICKETKEEPER BATSMAN', 'RR'),
('SHIMRON HETMYER', 14, 70, 0, 'LEFT HAND BATSMAN', 'RR'),
('TRENT BOULT', 18, 0, 7, 'LEFT ARM FAST BOWLER', 'RR'),
('DHRUV JUREL', 21, 50, 0, 'RIGHT HAND BATSMAN', 'RR'),
('ROVMAN POWELL', 22, 37, 0, 'RIGHT HAND BATSMAN', 'RR'),
('JOS BUTTLER', 63, 250, 0, 'RIGHT HAND BATSMAN', 'RR'),
('RAVICHANDRAN ASWIN', 99, 53, 1, 'RIGHT HAND BATSMAN, ', 'RR'),
('YASHASVI JAISWAL', 121, 0, 0, 'LEFT HAND BATSMAN', 'RR');

-- --------------------------------------------------------

--
-- Table structure for table `srh`
--

CREATE TABLE `srh` (
  `PLAYER_NAME` varchar(20) DEFAULT NULL,
  `JERSEY_NO` int(11) NOT NULL,
  `RUNS` int(11) DEFAULT NULL,
  `WICKETS` int(11) DEFAULT NULL,
  `PLAYER_ROLE` varchar(20) DEFAULT NULL,
  `TEAM_NAME` varchar(20) DEFAULT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci;

--
-- Dumping data for table `srh`
--

INSERT INTO `srh` (`PLAYER_NAME`, `JERSEY_NO`, `RUNS`, `WICKETS`, `PLAYER_ROLE`, `TEAM_NAME`) VALUES
('ABHISEKH SHARMA', 4, 211, 0, 'LEFT HAND BATSMAN, L', 'SRH'),
('AIDEN MARKARAM', 7, 159, 0, 'RIGHT HAND BATSMAN', 'SRH'),
('TRAVIS HEAD', 12, 235, 0, 'LEFT HAND BATSMAN', 'SRH'),
('BHUVANESHWAR KUMAR', 15, 6, 3, 'RIGHT ARM-MEDIUM FAS', 'SRH'),
('MAYANK AGARWAL', 16, 59, 0, 'RIGHT HAND BATSMAN', 'SRH'),
('SHABAZ AHMED', 21, 70, 3, 'LEFT HAND BATSMAN, L', 'SRH'),
('MARCO JANSEN', 23, 1, 0, 'LEFT HAND BATSMAN, L', 'SRH'),
('PAT CUMMINS', 30, 5, 9, 'RIGHT HANDED BATSMAN', 'SRH'),
('NATRAJAN', 44, 0, 6, 'LEFT ARM MEDIUM-FAST', 'SRH'),
('HEINRICH KLASEEN', 45, 253, 0, 'WICKETKEEPER BATSMAN', 'SRH'),
('RAHUL TRIPATHI', 52, 31, 0, 'RIGHT HAND BATSMAN', 'SRH');

-- --------------------------------------------------------

--
-- Table structure for table `team_table`
--

CREATE TABLE `team_table` (
  `TEAM_NAME` varchar(20) NOT NULL,
  `OWNER_NAME` varchar(20) DEFAULT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci;

--
-- Dumping data for table `team_table`
--

INSERT INTO `team_table` (`TEAM_NAME`, `OWNER_NAME`) VALUES
('CSK', 'INDIA CEMENTS'),
('DC', 'GMR GROUP'),
('GT', 'CVC CAPITAL'),
('KKR', 'RED CHILLIES'),
('LSG', 'RP SANJEEV GRP'),
('MI', 'RELIANCE'),
('PBKS', 'PREITY ZINTA'),
('RCB', 'UNITED SPIRITS'),
('RR', 'BLEAHEIM CHALCOT'),
('SRH', 'SUN TV');

-- --------------------------------------------------------

--
-- Structure for view `allrounder_list`
--
DROP TABLE IF EXISTS `allrounder_list`;

CREATE ALGORITHM=UNDEFINED DEFINER=`root`@`localhost` SQL SECURITY DEFINER VIEW `allrounder_list`  AS SELECT `all_players`.`PLAYER_NAME` AS `PLAYER_NAME`, `all_players`.`JERSEY_NO` AS `JERSEY_NO`, `all_players`.`TEAM_NAME` AS `TEAM_NAME`, `all_players`.`RUNS` AS `RUNS`, `all_players`.`WICKETS` AS `WICKETS` FROM (select `rcb`.`PLAYER_NAME` AS `PLAYER_NAME`,`rcb`.`JERSEY_NO` AS `JERSEY_NO`,`rcb`.`TEAM_NAME` AS `TEAM_NAME`,`rcb`.`RUNS` AS `RUNS`,`rcb`.`WICKETS` AS `WICKETS` from `rcb` union all select `csk`.`PLAYER_NAME` AS `PLAYER_NAME`,`csk`.`JERSEY_NO` AS `JERSEY_NO`,`csk`.`TEAM_NAME` AS `TEAM_NAME`,`csk`.`RUNS` AS `RUNS`,`csk`.`WICKETS` AS `WICKETS` from `csk` union all select `dc`.`PLAYER_NAME` AS `PLAYER_NAME`,`dc`.`JERSEY_NO` AS `JERSEY_NO`,`dc`.`TEAM_NAME` AS `TEAM_NAME`,`dc`.`RUNS` AS `RUNS`,`dc`.`WICKETS` AS `WICKETS` from `dc` union all select `mi`.`PLAYER_NAME` AS `PLAYER_NAME`,`mi`.`JERSEY_NO` AS `JERSEY_NO`,`mi`.`TEAM_NAME` AS `TEAM_NAME`,`mi`.`RUNS` AS `RUNS`,`mi`.`WICKETS` AS `WICKETS` from `mi` union all select `gt`.`PLAYER_NAME` AS `PLAYER_NAME`,`gt`.`JERSEY_NO` AS `JERSEY_NO`,`gt`.`TEAM_NAME` AS `TEAM_NAME`,`gt`.`RUNS` AS `RUNS`,`gt`.`WICKETS` AS `WICKETS` from `gt` union all select `lsg`.`PLAYER_NAME` AS `PLAYER_NAME`,`lsg`.`JERSEY_NO` AS `JERSEY_NO`,`lsg`.`TEAM_NAME` AS `TEAM_NAME`,`lsg`.`RUNS` AS `RUNS`,`lsg`.`WICKETS` AS `WICKETS` from `lsg` union all select `rr`.`PLAYER_NAME` AS `PLAYER_NAME`,`rr`.`JERSEY_NO` AS `JERSEY_NO`,`rr`.`TEAM_NAME` AS `TEAM_NAME`,`rr`.`RUNS` AS `RUNS`,`rr`.`WICKETS` AS `WICKETS` from `rr` union all select `kkr`.`PLAYER_NAME` AS `PLAYER_NAME`,`kkr`.`JERSEY_NO` AS `JERSEY_NO`,`kkr`.`TEAM_NAME` AS `TEAM_NAME`,`kkr`.`RUNS` AS `RUNS`,`kkr`.`WICKETS` AS `WICKETS` from `kkr` union all select `pbks`.`PLAYER_NAME` AS `PLAYER_NAME`,`pbks`.`JERSEY_NO` AS `JERSEY_NO`,`pbks`.`TEAM_NAME` AS `TEAM_NAME`,`pbks`.`RUNS` AS `RUNS`,`pbks`.`WICKETS` AS `WICKETS` from `pbks` union all select `srh`.`PLAYER_NAME` AS `PLAYER_NAME`,`srh`.`JERSEY_NO` AS `JERSEY_NO`,`srh`.`TEAM_NAME` AS `TEAM_NAME`,`srh`.`RUNS` AS `RUNS`,`srh`.`WICKETS` AS `WICKETS` from `srh`) AS `all_players` WHERE `all_players`.`RUNS` >= 50 AND `all_players`.`WICKETS` >= 1 ORDER BY `all_players`.`RUNS`+ `all_players`.`WICKETS` * 10 DESC LIMIT 0, 10 ;

-- --------------------------------------------------------

--
-- Structure for view `orange_cap`
--
DROP TABLE IF EXISTS `orange_cap`;

CREATE ALGORITHM=UNDEFINED DEFINER=`root`@`localhost` SQL SECURITY DEFINER VIEW `orange_cap`  AS SELECT `all_players`.`PLAYER_NAME` AS `PLAYER_NAME`, `all_players`.`JERSEY_NO` AS `JERSEY_NO`, `all_players`.`RUNS` AS `RUNS`, `all_players`.`TEAM_NAME` AS `TEAM_NAME` FROM (select `rcb`.`PLAYER_NAME` AS `PLAYER_NAME`,`rcb`.`JERSEY_NO` AS `JERSEY_NO`,`rcb`.`RUNS` AS `RUNS`,`rcb`.`TEAM_NAME` AS `TEAM_NAME` from `rcb` union all select `csk`.`PLAYER_NAME` AS `PLAYER_NAME`,`csk`.`JERSEY_NO` AS `JERSEY_NO`,`csk`.`RUNS` AS `RUNS`,`csk`.`TEAM_NAME` AS `TEAM_NAME` from `csk` union all select `dc`.`PLAYER_NAME` AS `PLAYER_NAME`,`dc`.`JERSEY_NO` AS `JERSEY_NO`,`dc`.`RUNS` AS `RUNS`,`dc`.`TEAM_NAME` AS `TEAM_NAME` from `dc` union all select `mi`.`PLAYER_NAME` AS `PLAYER_NAME`,`mi`.`JERSEY_NO` AS `JERSEY_NO`,`mi`.`RUNS` AS `RUNS`,`mi`.`TEAM_NAME` AS `TEAM_NAME` from `mi` union all select `gt`.`PLAYER_NAME` AS `PLAYER_NAME`,`gt`.`JERSEY_NO` AS `JERSEY_NO`,`gt`.`RUNS` AS `RUNS`,`gt`.`TEAM_NAME` AS `TEAM_NAME` from `gt` union all select `lsg`.`PLAYER_NAME` AS `PLAYER_NAME`,`lsg`.`JERSEY_NO` AS `JERSEY_NO`,`lsg`.`RUNS` AS `RUNS`,`lsg`.`TEAM_NAME` AS `TEAM_NAME` from `lsg` union all select `rr`.`PLAYER_NAME` AS `PLAYER_NAME`,`rr`.`JERSEY_NO` AS `JERSEY_NO`,`rr`.`RUNS` AS `RUNS`,`rr`.`TEAM_NAME` AS `TEAM_NAME` from `rr` union all select `kkr`.`PLAYER_NAME` AS `PLAYER_NAME`,`kkr`.`JERSEY_NO` AS `JERSEY_NO`,`kkr`.`RUNS` AS `RUNS`,`kkr`.`TEAM_NAME` AS `TEAM_NAME` from `kkr` union all select `pbks`.`PLAYER_NAME` AS `PLAYER_NAME`,`pbks`.`JERSEY_NO` AS `JERSEY_NO`,`pbks`.`RUNS` AS `RUNS`,`pbks`.`TEAM_NAME` AS `TEAM_NAME` from `pbks` union all select `srh`.`PLAYER_NAME` AS `PLAYER_NAME`,`srh`.`JERSEY_NO` AS `JERSEY_NO`,`srh`.`RUNS` AS `RUNS`,`srh`.`TEAM_NAME` AS `TEAM_NAME` from `srh`) AS `all_players` ORDER BY `all_players`.`RUNS` DESC LIMIT 0, 10 ;

-- --------------------------------------------------------

--
-- Structure for view `purple_cap`
--
DROP TABLE IF EXISTS `purple_cap`;

CREATE ALGORITHM=UNDEFINED DEFINER=`root`@`localhost` SQL SECURITY DEFINER VIEW `purple_cap`  AS SELECT `all_players`.`PLAYER_NAME` AS `PLAYER_NAME`, `all_players`.`JERSEY_NO` AS `JERSEY_NO`, `all_players`.`WICKETS` AS `WICKETS`, `all_players`.`TEAM_NAME` AS `TEAM_NAME` FROM (select `rcb`.`PLAYER_NAME` AS `PLAYER_NAME`,`rcb`.`JERSEY_NO` AS `JERSEY_NO`,`rcb`.`WICKETS` AS `WICKETS`,`rcb`.`TEAM_NAME` AS `TEAM_NAME` from `rcb` union all select `csk`.`PLAYER_NAME` AS `PLAYER_NAME`,`csk`.`JERSEY_NO` AS `JERSEY_NO`,`csk`.`WICKETS` AS `WICKETS`,`csk`.`TEAM_NAME` AS `TEAM_NAME` from `csk` union all select `dc`.`PLAYER_NAME` AS `PLAYER_NAME`,`dc`.`JERSEY_NO` AS `JERSEY_NO`,`dc`.`WICKETS` AS `WICKETS`,`dc`.`TEAM_NAME` AS `TEAM_NAME` from `dc` union all select `mi`.`PLAYER_NAME` AS `PLAYER_NAME`,`mi`.`JERSEY_NO` AS `JERSEY_NO`,`mi`.`WICKETS` AS `WICKETS`,`mi`.`TEAM_NAME` AS `TEAM_NAME` from `mi` union all select `gt`.`PLAYER_NAME` AS `PLAYER_NAME`,`gt`.`JERSEY_NO` AS `JERSEY_NO`,`gt`.`WICKETS` AS `WICKETS`,`gt`.`TEAM_NAME` AS `TEAM_NAME` from `gt` union all select `lsg`.`PLAYER_NAME` AS `PLAYER_NAME`,`lsg`.`JERSEY_NO` AS `JERSEY_NO`,`lsg`.`WICKETS` AS `WICKETS`,`lsg`.`TEAM_NAME` AS `TEAM_NAME` from `lsg` union all select `rr`.`PLAYER_NAME` AS `PLAYER_NAME`,`rr`.`JERSEY_NO` AS `JERSEY_NO`,`rr`.`WICKETS` AS `WICKETS`,`rr`.`TEAM_NAME` AS `TEAM_NAME` from `rr` union all select `kkr`.`PLAYER_NAME` AS `PLAYER_NAME`,`kkr`.`JERSEY_NO` AS `JERSEY_NO`,`kkr`.`WICKETS` AS `WICKETS`,`kkr`.`TEAM_NAME` AS `TEAM_NAME` from `kkr` union all select `pbks`.`PLAYER_NAME` AS `PLAYER_NAME`,`pbks`.`JERSEY_NO` AS `JERSEY_NO`,`pbks`.`WICKETS` AS `WICKETS`,`pbks`.`TEAM_NAME` AS `TEAM_NAME` from `pbks` union all select `srh`.`PLAYER_NAME` AS `PLAYER_NAME`,`srh`.`JERSEY_NO` AS `JERSEY_NO`,`srh`.`WICKETS` AS `WICKETS`,`srh`.`TEAM_NAME` AS `TEAM_NAME` from `srh`) AS `all_players` ORDER BY `all_players`.`WICKETS` DESC LIMIT 0, 10 ;

-- --------------------------------------------------------

--
-- Structure for view `qualifier_fixtures`
--
DROP TABLE IF EXISTS `qualifier_fixtures`;

CREATE ALGORITHM=UNDEFINED DEFINER=`root`@`localhost` SQL SECURITY DEFINER VIEW `qualifier_fixtures`  AS SELECT concat('QUALIFIER ',`q1`.`team1`,' VS ',`q1`.`team2`) AS `FIXTURE` FROM (select `pt1`.`TEAM_NAME` AS `team1`,`pt2`.`TEAM_NAME` AS `team2` from (`point_table` `pt1` join `point_table` `pt2`) where `pt1`.`TEAM_NAME` < `pt2`.`TEAM_NAME` order by `pt1`.`POINTS` desc,`pt2`.`POINTS` desc limit 1) AS `q1`union all select concat('ELIMINATOR 1 ',`q2`.`team1`,' VS ',`q2`.`team2`) AS `FIXTURE` from (select `pt1`.`TEAM_NAME` AS `team1`,`pt2`.`TEAM_NAME` AS `team2` from (`point_table` `pt1` join `point_table` `pt2`) where `pt1`.`TEAM_NAME` < `pt2`.`TEAM_NAME` order by `pt1`.`POINTS` desc,`pt2`.`POINTS` desc limit 1,1) `q2`  ;

--
-- Indexes for dumped tables
--

--
-- Indexes for table `csk`
--
ALTER TABLE `csk`
  ADD PRIMARY KEY (`JERSEY_NO`),
  ADD KEY `TEAM_NAME` (`TEAM_NAME`);

--
-- Indexes for table `dc`
--
ALTER TABLE `dc`
  ADD PRIMARY KEY (`JERSEY_NO`),
  ADD KEY `TEAM_NAME` (`TEAM_NAME`);

--
-- Indexes for table `gt`
--
ALTER TABLE `gt`
  ADD PRIMARY KEY (`JERSEY_NO`),
  ADD KEY `TEAM_NAME` (`TEAM_NAME`);

--
-- Indexes for table `kkr`
--
ALTER TABLE `kkr`
  ADD PRIMARY KEY (`JERSEY_NO`),
  ADD KEY `TEAM_NAME` (`TEAM_NAME`);

--
-- Indexes for table `lsg`
--
ALTER TABLE `lsg`
  ADD PRIMARY KEY (`JERSEY_NO`),
  ADD KEY `TEAM_NAME` (`TEAM_NAME`);

--
-- Indexes for table `mi`
--
ALTER TABLE `mi`
  ADD PRIMARY KEY (`JERSEY_NO`),
  ADD KEY `TEAM_NAME` (`TEAM_NAME`);

--
-- Indexes for table `pbks`
--
ALTER TABLE `pbks`
  ADD PRIMARY KEY (`JERSEY_NO`),
  ADD KEY `TEAM_NAME` (`TEAM_NAME`);

--
-- Indexes for table `point_table`
--
ALTER TABLE `point_table`
  ADD PRIMARY KEY (`TEAM_NAME`);

--
-- Indexes for table `rcb`
--
ALTER TABLE `rcb`
  ADD PRIMARY KEY (`JERSEY_NO`),
  ADD KEY `TEAM_NAME` (`TEAM_NAME`);

--
-- Indexes for table `rr`
--
ALTER TABLE `rr`
  ADD PRIMARY KEY (`JERSEY_NO`),
  ADD KEY `TEAM_NAME` (`TEAM_NAME`);

--
-- Indexes for table `srh`
--
ALTER TABLE `srh`
  ADD PRIMARY KEY (`JERSEY_NO`),
  ADD KEY `TEAM_NAME` (`TEAM_NAME`);

--
-- Indexes for table `team_table`
--
ALTER TABLE `team_table`
  ADD PRIMARY KEY (`TEAM_NAME`);

--
-- Constraints for dumped tables
--

--
-- Constraints for table `csk`
--
ALTER TABLE `csk`
  ADD CONSTRAINT `csk_ibfk_1` FOREIGN KEY (`TEAM_NAME`) REFERENCES `team_table` (`TEAM_NAME`);

--
-- Constraints for table `dc`
--
ALTER TABLE `dc`
  ADD CONSTRAINT `dc_ibfk_1` FOREIGN KEY (`TEAM_NAME`) REFERENCES `team_table` (`TEAM_NAME`);

--
-- Constraints for table `gt`
--
ALTER TABLE `gt`
  ADD CONSTRAINT `gt_ibfk_1` FOREIGN KEY (`TEAM_NAME`) REFERENCES `team_table` (`TEAM_NAME`);

--
-- Constraints for table `kkr`
--
ALTER TABLE `kkr`
  ADD CONSTRAINT `kkr_ibfk_1` FOREIGN KEY (`TEAM_NAME`) REFERENCES `team_table` (`TEAM_NAME`);

--
-- Constraints for table `lsg`
--
ALTER TABLE `lsg`
  ADD CONSTRAINT `lsg_ibfk_1` FOREIGN KEY (`TEAM_NAME`) REFERENCES `team_table` (`TEAM_NAME`);

--
-- Constraints for table `mi`
--
ALTER TABLE `mi`
  ADD CONSTRAINT `mi_ibfk_1` FOREIGN KEY (`TEAM_NAME`) REFERENCES `team_table` (`TEAM_NAME`);

--
-- Constraints for table `pbks`
--
ALTER TABLE `pbks`
  ADD CONSTRAINT `pbks_ibfk_1` FOREIGN KEY (`TEAM_NAME`) REFERENCES `team_table` (`TEAM_NAME`);

--
-- Constraints for table `point_table`
--
ALTER TABLE `point_table`
  ADD CONSTRAINT `point_table_ibfk_1` FOREIGN KEY (`TEAM_NAME`) REFERENCES `team_table` (`TEAM_NAME`);

--
-- Constraints for table `rcb`
--
ALTER TABLE `rcb`
  ADD CONSTRAINT `rcb_ibfk_1` FOREIGN KEY (`TEAM_NAME`) REFERENCES `team_table` (`TEAM_NAME`);

--
-- Constraints for table `rr`
--
ALTER TABLE `rr`
  ADD CONSTRAINT `rr_ibfk_1` FOREIGN KEY (`TEAM_NAME`) REFERENCES `team_table` (`TEAM_NAME`);

--
-- Constraints for table `srh`
--
ALTER TABLE `srh`
  ADD CONSTRAINT `srh_ibfk_1` FOREIGN KEY (`TEAM_NAME`) REFERENCES `team_table` (`TEAM_NAME`);
COMMIT;

/*!40101 SET CHARACTER_SET_CLIENT=@OLD_CHARACTER_SET_CLIENT */;
/*!40101 SET CHARACTER_SET_RESULTS=@OLD_CHARACTER_SET_RESULTS */;
/*!40101 SET COLLATION_CONNECTION=@OLD_COLLATION_CONNECTION */;
