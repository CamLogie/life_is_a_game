# Life is a Game
Building an application to help gamify some aspects of life. Planning on having different point systems that help you keep track of what you're doing well on and things that you need to improve


Running App:
1. Ensure your OS is using Python 3.10.4
2. Create a new virtual environment in the top level of this directory
3. Activate the virtual environment and install the requirements.txt files
4. Export the following variables to your shell:
    - `DATABASE_USER=<database_username>`
    - `DATABASE_PASSWORD=<password_for_username>`
    - `SEED_USER_PASSWORD=<password_for_seed_user>`
5. After all installations, run `flask --app life_is_a_game` init-db to initialize your database

Database Notes:
This program relies on postgres and pyscopg2 as its database and database adapter.

1. You may need to ensure that you have a database named life_is_a_game on your machine
2. You will need to create a user for that database and allow that user to write to the database as well as:
    - `GRANT ALL ON SCHEMA public TO <database_username>`

Scripts:

I have included some simple shell scripts that can be run to test the app, run it in debug mode, and run it normally. They are under life_is_a_game/scripts/