Currently there is no deployment, the project is only available locally in its current configuration. 

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
