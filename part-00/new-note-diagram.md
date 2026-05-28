sequenceDiagram
    participant browser
    participant server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note
    server-->>browser: HTTP status code 302 URL redirect
    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/notes
    server-->>browser: main.css
    server-->>browser: main.js
    server-->>browser: data.json

