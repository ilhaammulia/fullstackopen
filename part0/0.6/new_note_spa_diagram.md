sequenceDiagram
participant browser
participant server

    Note right of browser: Redraw notes when user click save button

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: {"message":"note created"}
    deactivate server
