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


![Screenshot (43)](https://github.com/user-attachments/assets/e9c737fb-9b44-4448-8cfa-4d39d4bb3471)

• Contains the core elements of the Interfact admin dashboard, including:

    - All .tsx pages for interactable elements 
    - DAO/Firebase files
    - Files for system font
    - Typescript hooks for user feedback and Intersection data
    - + other files such as the Dockerfile, tsconfig & firebaseconfig files, and more. 


# Explaining config files

• babel.config.js: Configures the JS Babel compiler to work with a react project & typescript.

• jest.config.ts: See code comments [HERE](https://github.com/AceLeft/Interfact-Admin-Dashboard/blob/main/interfact-admin-dashboard/jest.config.ts)

• next.config.ts: Sets strict mode in react off.

# How to replicate Via Docker
1. Clone github in a gitbash terminal via `git clone https://github.com/AceLeft/Interfact-Admin-Dashboard`
2. Get VSCode for your computer via https://code.visualstudio.com/
3. Download [Docker Desktop](https://www.docker.com/products/docker-desktop/) for your OS
4. Download [Node.js](https://nodejs.org/en) of version 22 or higher. You can check what version you have by entering `node -v` into a terminal.
   * If you have an earlier version of node, download a newer one to overwrite it
5. In the terminal in VSCode, enter the `command docker build -t dashboard-image .`
   * This creates a new image of the name "dashboard-image"
   * Be sure to include the period at the end
   * The initial build will be slow, around 3 minutes, but it will speed up after the first time
6. In the terminal, run `docker run -d -p 3000:3000 dashboard-image`
7. Visit http://localhost:3000/ to ensure that it is running

# How to run tests
  To run system tests, type "npm run test" into the project terminal.

