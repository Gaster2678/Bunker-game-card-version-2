This Python code manages a SQLite database for a game called "Bunker." It includes functions for creating tables, inserting data, and performing various operations on the database.

Database Creation:

create_bd class contains functions to create five tables in the database:
Players: Stores player information (user ID, play ID, player ID, send ID, and vote).
Player_Cards: Stores player card details (profession, biology, health, hobby, luggage, evidence, and special conditions).
Player_Cards_check: Stores a copy of player card details with initial values set to 0.
Bunker_Cards: Stores bunker card details (disasters, danger level, and seven bunker cards).
Last_value: Stores the last assigned user ID and play room ID.
Data Insertion:

test_bd class contains functions to insert data into the database:
test_bd_Players: Inserts a new player into the Players table.
test_bd_Player_Cards: Inserts player card details into the Player_Cards table.
test_bd_Player_Cards_check: Inserts initial values into the Player_Cards_check table.
test_bd_Bunker_Cards: Inserts bunker card details into the Bunker_Cards table.
test_bd_Last_value: Inserts the last assigned user ID and play room ID into the Last_value table.
test_bd_all: Inserts all necessary data for a new game session.
Database Operations:

Jobs_bd class contains functions for managing game-related operations:
add_play_and_room: Creates a new game session and inserts data for the first player.
add_play: Adds a new player to an existing game session.
Development Functions:

dev_jobs_bd class contains functions for managing database values:
last_value_player: Gets the last assigned user ID.
last_value_room: Gets the last assigned play room ID.
next_value_player: Increments the last assigned user ID.
next_value_room: Increments the last assigned play room ID.
Database Reload:

reload_bd function:
Drops all tables in the database.
Recreates all tables.
Inserts sample data for testing purposes.
This code provides a comprehensive set of functions for managing the database for the "Bunker" game, allowing for easy data insertion, retrieval, and manipulation