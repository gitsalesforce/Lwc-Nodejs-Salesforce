# Demo: Lightning Out + Visualforce/Node.js + LWC/Aura (Node.js Server)

# What is this?
This is one of two repos that will help you get started with **Lightning Out** in Visualforce and Node.js application to render **Lightning Components** both **Aura** and **LWC**.

> This repo contains the Node.js server built using Typescript, express and ejs.

# How to use it?
Make sure you get both repos, then get the scratch org ready and execute the Node.js server.

## How to create the org?
- Create a scratch org by executing this command `./@ELTOROIT/scripts/CreateOrg.sh`
- At the end of that script, it creates the pasword for the user and displays some important information. Make sure you keep that open (if you close it, you can execute `sfdx force:user:display`).
- On the Scratch org that was created, reset the security token for API connections.

# How to configure the Node.js application?
- First, rebuild the **node_modules** folder by executing `npm install`
- Open VS Code and find the `.env` file
- Update the content using the information at the end of the script that creates the scrach org and the security token.
-  Start the web server, by hitting `F5`
- Once it has compiled, open a web browser and navigate to either `http://localhost:5000` or `https://localhost:5001`

**Note:** The Node.js web server is using a self-signed certificate which is required for HTTPS, but obviously is not secured. When you open the "secured" site, the browser is going to report a warning but you can bypass it and get to the content. When you deploy this to a real server, and use a good certificate, this problem will not happen any more.
