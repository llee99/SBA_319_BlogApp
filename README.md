# SBA 319: COMMUNITY BLOG APP

1. In this project I am creating a mock community blog page, where user can post about a variety of topics and other users will be able to comment down below, as well as the original author. A major update in the future would be a an account creation feature that would provide user authetication for users as well as distinguish between verified, unverified, and anonymous accounts.

2. I will utilize the MongoDB cluster that we made during class (Cluster0) to provide permanent CRUD functionality to the data (posts, comments, insertions/deletions).

3. Two folders separate the client side and server side functionality. After running the terminal commands to install an earlier version of Node in both directories, starting the Express server, and also importing the React module, I created the server files to connect the database via the ATLAS_URI string in a .env file, and began writing the routes for get, post, patch, and delete.

4. In the index.mjs file I called the middleware function for the routes path as well as error handling routes using app.use, and used app.listen to start the Express server

5. In the client side app directory, I created two sub directories, public (to store png files, icons, and the template html file index.html) and src (contains the sub-directories: components and pages, as well as the HTML embedded JS files App and index). The App file makes use of the leafygreen-provider package for user interaction related information about our components.

6. The components sub directory makes use of the ...props feature as well as embedded CSS to create wrapper components which will be used to determine the aesthetic of category logos on each page. The Header, Layout, and Navigation js files all provide wrapper functionality through the imported React components as well as the public leafygreen-ui React UI kit. The PostSummary file provides a template for a concise view of each Question/Post.

7. The pages sub directory contains js files that return React fragments, a feature that allows multiple return elements froma single component by grouping child nodes into lists. The js files also make use of the App.tsx file by exporting the default App() function.

8. Additional external CSS was implemented through the styles.css file. Compatability issues existed with framework versions that were outdated, so the specific versions of frameworks and languages were used to maintain cohesiveness throughout the project.


Start the Express server with the following commands:
cd server
npm install
npm run dev

Then in a new terminal window, start the client-side React app with these commands:
cd app
npm install
npm start# SBA_319
