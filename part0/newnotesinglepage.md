```mermaid
    sequenceDiagram
        participant browser
        participant server

        Note right of browser: User creates a new note and click Save button

        browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
        activate server
        server-->>browser: new_note_spa json is sent 
        deactivate server

        Note right of browser: new_note_spa json comtains the new note user entered

```