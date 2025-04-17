Currently there is no external deployment, the project is only available locally in its current configuration. 

# Running Locally:

1. Clone github in a gitbash terminal via `git clone https://github.com/AceLeft/Interfact-Admin-Dashboard`
2. Get VSCode for your computer via https://code.visualstudio.com/
3. Open the dashboard folder in VSCode. Then, open a terminal in VSCode. First, make sure you cd into /interfact-admin-dashboard/. You may ensure you are in the right folder by typing `ls` into the terminal; you should see many .js and .ts files. Then, run `npm install` to install all of the project's dependencies.
5. Make sure your node.js is > 18.18, if not download from https://nodejs.org/en
6. Download & setup the fontawesome packages by following the instructions on: `https://docs.fontawesome.com/web/use-with/react`
7. Install MySQL (Guide: `https://docs.fontawesome.com/web/use-with/react`)
8. Create a MySQL account, and type your password into the .env file variable "DB_Pass" on line 10.
9. Type "npm install mysql2" into the terminal to install the necessary components for the mySQL database
10. In the terminal, type "npm run dev", and wait for the dashboard to compile.
11. On a browser tab on your machine, type "http://localhost:3000" into the address bar.

## .env
In order to run the project with your own MySQL, database, and python script, a `.env` file is required. This is a file located at the root directory (located on the same level as `package.json`) that has the name `.env`.
The following values are required for the project to run. The `ALL_CAPS` values may not be changed; the correct values are added after the =.
`NEXT_PUBLIC_FIREBASE_API_KEY=` <- This is the key for your Firebase API 
`NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=` <- This is the domain name for your Firebase app
`NEXT_PUBLIC_FIREBASE_PROJECT_ID=` <- This is the ID of your Firebase project
`NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=` <- This is the domain for your storage Firebase app
`NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=`
`NEXT_PUBLIC_FIREBASE_APP_ID=`
`DB_HOST=` <- This is the host for your MySQL. For example, localhost
`DB_USER=` <- This is the user of your MySQL. For exmaple, root
`DB_PASS=` <- This is your MySQL password
`DB_NAME=` <- This is the name of your MySQL database
`DB_PORT=` <- This is the desired port for you MySQL database
`NEXT_PUBLIC_RETRAIN_PYTHON_FILE=` <- This is the location on your computer of the python script that will retrain the train detecting system. If you do not have one, you may use `src/app/api/python/placeholder.py` as a nonfunctioning placeholder.
