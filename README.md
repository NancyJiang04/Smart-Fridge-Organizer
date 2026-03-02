# Smart-Fridge-Organizer
Smart Fridge Organizer is a website that allows users to keep track of items stored in their fridge and freezer. The app helps users reduce food waste by showing expiry warnings, organising items by location (fridge and freezer), and providing simple recipe suggestions based on available ingredients. The project is built by using Python, Flask, SQL, HTML and Bootstrap.


# 2. Purpose of this Project
The idea came from a daily problem my friend and I face: we constantly forget what we bought, what we still have and what has already expired. Food ends up wasted or duplicated simply because we lose track. This website wants to solve this by providing a clear digital inventory where users can record items, monitor expiry dates and see what they can cook based on their ingredients.

# 3. Install and Run the Project
1. Download or unzip the project folder

2. Install all required Python packages using:

    pip install -r requirements.txt

3. Make sure you are inside the project folder (smart-fridge/).

4. Start the Flask server by running:

    flask run

5. A link will appear in the terminal. Open it in your browser to access the application.

# 4. Project (file) Structure
smart-fridge/
---app.py # Main Application for Flask
---fridge.db # SQLite database
---requirements.txt
---static/
----fridge_bear.png # Image on Homepage
---templates/
----add.html
----edit.html
----index.html
----layout.html
----login.html
----recipes.html
----register.html

# 5.Database Structure
The project uses SQLite database (fridge.db), which contain 2 tables:
[table 1: users]
- id
- username
- hash
[table 2: items]
- id
- user_id
- name
- quantity
- category
- location
- purchase_date
- expiry_date

# 6. How to use the Smart Fridge Organizer
1. Register for an account on the Register page
2. Log in using your username and password
3. After logging in, you will see two tables: Fridge Items and Freezer Items
4. Click "Add Item" to insert new food entries
5. Each item can be edited or deleted using the buttons in the table
6. Click "Recipes" to see which meals (only contain several simple recipes) you can make using your current ingredients
7. Use the "Logout" button to end your session

# 7. Youtube Video URL
https://youtu.be/fSKiUhQm7ks
