# fso-part0

sequenceDiagram
  participant browser
  participant server

  
  browser->> server: POST input value
  activate server
  server->>browser: response header
  deactivate server

  Input value gets stored in an array and JS file creates a child element to the list and makes it appear on the website without refreshing the page.
  

  
