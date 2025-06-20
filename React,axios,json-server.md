# Notes: React + axios + json-server Setup

1 **What is a React project?**
  * React is a JavaScript library for building user interfaces (UI)
  * It controls:
    * What the UI looks like
    * How the UI responds to user actions
  * In a React project, you write components, which are reusable building blocks that define how part of the UI behaves and looks

2 **What are db.json and json-server?**
  * db.json is a plain JSON file that holds mock data (e.g., a list of members)
  * json-server is a tool that automatically creates a fake REST API(Representational State Transfer) based on the content of db.json
  * To start it:
                npx json-server --watch db.json --port 3100 &nbsp; **(json-server.json won't change the start code)**
  * This creates an API endpoint like:
                                     http://localhost:3100/members
  * Benefit: You can simulate a backend without writing any server code

3 **What is axios?**
  * axios is a JavaScript library for sending HTTP requests (GET, POST, etc.)
  * Basic usage:
               axios.get("http://localhost:3100/members")
  * Features:
    * Supports Promise and async/await
    * Simplifies data fetching and error handling

4 **How do React, axios, and json-server work together?**
  The typical workflow:
  1. A button is displayed in a React component
  2. When the user clicks the button, it triggers a function (e.g., onFetchClick)
  3. The function sends a GET request using axios to the json-server API
  4. json-server responds with data from db.json
  5. The React component receives the data and updates the state with setMembers()
  6. React automatically re-renders the UI to display the updated data

5 **Why is this workflow important?**
  * In real-world projects, front-end apps often need to communicate with backend APIs
  * Understanding this pattern helps you manage data flow between frontend and backend
  * Using a mock server like json-server lets you:
    * Test your front-end without needing a real backend
    * Build and debug early without waiting for backend development





  
