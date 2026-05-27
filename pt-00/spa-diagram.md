sequenceDiagram
    participant browser
    participant server

    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/spa
    server-->>browser: spa html
    server-->>browser: main.css
    server-->>browser: spa.js
    server-->>browser: data.json
