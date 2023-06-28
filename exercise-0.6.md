sequenceDiagram
  participant browser
  participant server

  browser->> server: POST input value
  activate server
  server->> browser: response header
  deactivate server 

  The main difference betwween adding a note in traditional web app and adding a note in SPA is that traditional web app needs to refresh and get redirected whereas SPA changes its content dynamically with the help of JS.
