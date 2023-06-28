# fso-exercise-0.4

sequenceDiagram
  participant browser
  participant server

  browser->>server: POST the input value
  activate server
  server->>browser: response header
  deactivate server

  browser->> server: GET https://studies.cs.helsinki.fi/exampleapp/notes/
  activate server
  server->> browser: HTML document
  deactivate server

  browser->> server: GET https://studies.cs.helsinki.fi/exampleapp/notes/main.css
  activate server
  server->> browser: CSS file
  deactivate server

  browser->> server: GET https://studies.cs.helsinki.fi/exampleapp/notes/main.js
  activate server
  server->> browser: JS file
  deactivate server

  browser->> server: GET https://studies.cs.helsinki.fi/exampleapp/notes/data.json
  activate server
  server->>browser: json data
  deactivate server
  
