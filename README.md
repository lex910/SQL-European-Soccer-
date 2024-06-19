# SQL-European-Soccer-

Abstract: 
This project explores the European Soccer database using SQL and tableau to provide insights into trends. This project provides an explination of the data, how it was split up into tables, the relationships between the tables in an ER diagram, and lastly the questions and insights/visaulizations generated from the queries. 

Data Overview:
The data is sourced from Kaggle. There are 7 different data files. The files include country, league, match, player, playyer_attributes, team, and team_attributes. Country and league share id as a primary key to show the relationship of which leagues belong to which European country. League and match share country_id as a primary key. Player and player_attribute are linked by player_api_id, while team and team_attributes have team_api_id as primary keys. Overall the data shows the different leagues in several European countries, specific match details, player demographics, player specific match statistics, teams, and individual team attributes.

ER Diagram:
<img width="741" alt="Screenshot 2024-06-19 at 9 19 39 AM" src="https://github.com/lex910/SQL-European-Soccer-/assets/101606445/c651ef0f-adb0-47fa-a72e-1152186afdf3">

Discussion of conversion of the dataset into tables:
In order to convert the dataset into tables, it was first necessary to understand all of the variables present in the dataset and how they were related to one another. The dataset was easily able to be split up into distinct variables that contained appropriate data specific to the individual table. The dataset could be split up into 7 tables with specifics about country, league, match, player, player attributes, team, and team attributes data.
After the database was split up into 7 tables with the specific entities becoming the columns, relationships between table entities needed to be established to link the tables to one another. Primary keys are foreign keys linked the tables together based on similar attributes that appear between two tables.
The last step of converting the dataset into tables was to populate them in MySQL. I was able to easily select the option to create a new schema and name the database appropriately. Once I refreshed the schemas I was able to see my new database and select tables. From here I used the Table Import Data Wizard to upload each CSV that was associated with each table. Here I was given the option to confirm the data types and select primary keys of each table.

Queries: 

# Question 1: Which leagues are in which European Country and what are the most popular leagues based on how many teams play in each league?

Insights: 
11 countries 
11 leagues 
Number of teams vary per league 
English Premier, France Ligue, Italy Serie A, Spain Liga: 20 teams 
Switzerland Super 9 teams

<img width="922" alt="Screenshot 2024-06-19 at 9 27 04 AM" src="https://github.com/lex910/SQL-European-Soccer-/assets/101606445/fe920f07-dda2-4c39-a38d-2e30d579ce92">

# Question 2: In the 2015/2016 season are the number of home and away games played consistent across leagues?

Insights: 
Within  each league every team played the same amount of home and away games

Spain LIGA, Scotland Premier, and Italy Serie A, Premier league, and France Ligue  had the most amount of matches: 19 home 19 away 

Poland Ekstraklasa and Belgium Jupiler had the least with 15 home, 15 away 

# Question 3: Which players have the highest max overall rating based off of their highest received rating over their career?

Insights: 
<img width="864" alt="Screenshot 2024-06-19 at 9 59 06 AM" src="https://github.com/lex910/SQL-European-Soccer-/assets/101606445/813d96dc-270c-48f6-a87b-ab522e6c8f1a">

# Question 4: Which teams had the most wins in each league during the 2015/2016 season?

Insights:
<img width="848" alt="Screenshot 2024-06-19 at 9 59 56 AM" src="https://github.com/lex910/SQL-European-Soccer-/assets/101606445/1594741e-ee18-4bb3-a10a-06987e4cca61">

# Question 5: What were the top scoring teams in each league during the most recent (2015/2016) season?

Insights:
Spain Liga: Barcelona, 112 goals 
France Ligue:Paris St. Germain, 102 goals  
Scotland Premier: Celtic, 93 goals 
Portugal Liga: SL Benfica, 88 goals 
Switzerland Super: FC Basel, 88 goals 
Netherlands Eredivisie: PSV, 88 goals 
Italy Serie A: Roma, 83 goals 
Germany Bundesliga: Dortmund, 82 goals 
England Premier: Manchester City, 71 goals 
Belgium Jupiler: Club Brugge, 64 goals 
Poland Ekstraklasa: Legia Warszawa, 58 goals 

# Question 6: Is there a home team advantage (on average more home team goals than away team goals) for each season?

Insights: 
<img width="868" alt="Screenshot 2024-06-19 at 10 00 49 AM" src="https://github.com/lex910/SQL-European-Soccer-/assets/101606445/feb9f9f8-cd40-4928-87c6-36643faf45a3">

# Question 7: Which teams are best defensively in each league given the number of goals conceded in the most recent season?

Insights: 
Spain Liga: Atletico Madrid
France Ligue:Losc Lille
Scotland Premier: Celtic (also most goals) 
Portugal Liga: Sporting CP
Switzerland Super: FC Basel (also most goals) 
Netherlands Eredivisie: Ajax
Italy Serie A: Juventus
Germany Bundesliga: FC Bayern Munich
England Premier: Manchester City (also most goals)
Belgium Jupiler: Club Brugge (also most goals) 
Poland Ekstraklasa: Piast Gliwice

# Question 8: What are the player attributes of the top 4 highest ranked players in European Soccer based off of most recent ratings?

Inisghts: 
<img width="867" alt="Screenshot 2024-06-19 at 10 01 44 AM" src="https://github.com/lex910/SQL-European-Soccer-/assets/101606445/7a1470ef-41b0-4462-93ea-0fae96eb4756">


