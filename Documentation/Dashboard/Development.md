# Manual Replication
1. Clone github in a gitbash terminal via `git clone https://github.com/AceLeft/Interfact-Admin-Dashboard`
2. Get VSCode for your computer via https://code.visualstudio.com/
3. Open the dashboard folder in VSCode. Then, open a terminal in VSCode. First, make sure you cd into /interfact-admin-dashboard/. You may ensure you are in the right folder by typing `ls` into the terminal; you should see many .js and .ts files. Then, run `npm install` to install all of the project's dependencies.
5. Make sure your node.js is > 18.18, if not download from https://nodejs.org/en
6. Download & setup the fontawesome packages by following the instructions on: `https://docs.fontawesome.com/web/use-with/react`
7. In the terminal, type "npm run dev", and wait for the dashboard to compile.
8. On a browser tab on your machine, type "http://localhost:3000" into the address bar.

# Folder Structure
![Screenshot (43)](https://github.com/user-attachments/assets/e3ad351f-0387-4019-bafd-1911021eb696)

- _mocks_ : Contains mock data for testing purposes
- _tests_ : System tests
-  public : Contains .webp images used in the system

src/app
![image](https://github.com/user-attachments/assets/093726f4-5722-4da7-89e4-9f1de76e603a)
• Contains the core elements of the Interfact admin dashboard, including:
    - All .tsx pages for interactable elements 
    - DAO/Firebase files
    - Files for system font
    - Typescript hooks for user feedback and Intersection data
    - + other files such as the Dockerfile, tsconfig & firebaseconfig files, and more. 


# Explaining config files

# How to replicate Via Docker
1. Clone github in a gitbash terminal via `git clone https://github.com/AceLeft/Interfact-Admin-Dashboard`
2. Get VSCode for your computer via https://code.visualstudio.com/
3. Download [Docker Desktop](https://www.docker.com/products/docker-desktop/) for your OS

# How to run tests & Interpret the results
  To run system tests, type "npm run test" into the project terminal.

