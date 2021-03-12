# Job-Tracker

**a. Description and working of the project:**
  * First of all, I have used python (IPythonNotebook), to read the .csv files. This python notebook takes care of resolving the job source from the url and                 dumping the data the database 'jobOpportunites.db'. There are two tables, 'JobBoards' that stores data from the json file and 'JobListings' for all the job listing and its source.For minimum overload, I have used sqlite3 as the database. In the file "Pathrise_Data_Preprocessing.ipynb", I have mentioned detailed comments on each step.
  
  * For the frontend part, I have used React.js to display the job sources and the job postings by the respective job source. I have used 'axios' to handle the backend api calls for data transfer.
  
  * For the backend part, I have used Node.js and Express.js to handle endpoints and GET/POST requests to and from both the tables.I have made use of 'url' node library to handle the POST request, parse the request query string and identify which job source was clicked on the UI. The sqlite query filters out the results if the Job Title is NULL or Company Name is Unknown or NULL.

b. **To run the app:**
  * Open Terminal/cmd.
  * Enter command following commands:
      * git clone https://github.com/RKBOSAMIA/Job-Tracker.git
      * cd Job-Tracker/backend
      * npm install express (this step is required if express.js is not installed)
      * npm start 
  * This will start the server on http://localhost:8000. This URL can be direct entered in a browser.
   
c. **Below is the list of dependencies for the project:**
  * Node server/backend dependencies.
    "dependencies": {
    "cors": "^2.8.5",
    "express": "^4.17.1",
    "morgan": "^1.10.0",
    "sqlite3": "^5.0.2"
  }
  * React / frontend dependencies.
    "dependencies": {
    "@material-ui/core": "^4.11.3",
    "@testing-library/jest-dom": "^5.11.9",
    "@testing-library/react": "^11.2.5",
    "@testing-library/user-event": "^12.8.3",
    "axios": "^0.21.1",
    "react": "^17.0.1",
    "react-dom": "^17.0.1",
    "react-router": "^5.2.0",
    "react-router-dom": "^5.2.0",
    "react-scripts": "4.0.3",
    "web-vitals": "^1.1.0"
  }
  * I have installed every thirs party library using the 'npm' command.
  
 d.**Publicly accessible URL**
  I have deployed the application on Heroku. The link to the app
  * [https://job-trackerr.herokuapp.com/](url)
 
 e. **Resolved job opportunities .csv file**
  * [https://github.com/RKBOSAMIA/Job-Tracker/blob/master/Files/resolvedJobOpportunities.csv](url)
 
 f. **Visualisation**
  * I have used python dictionary to count the total number of jobs each board and have dumped it to a json file. Here is the link to the file:
  [https://github.com/RKBOSAMIA/Job-Tracker/blob/master/Files/jobCounter.json](url)
