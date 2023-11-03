# Note-Taker Application



## Description

This is a note-taking application designed for small business owners to help them write and save notes. The application allows users to organize their thoughts and keep track of tasks they need to complete.

## User Story

As a small business owner, I want to be able to write and save notes so that I can organize my thoughts and keep track of tasks I need to complete.

## Acceptance Criteria

- The landing page should have a link to a notes page.
- Clicking on the link to the notes page should display a page with existing notes listed in the left-hand column.
- The page should have empty fields to enter a new note title and the note's text in the right-hand column.
- Entering a new note title and the note's text should make a Save icon appear in the navigation at the top of the page.
- Clicking on the Save icon should save the new note and display it in the left-hand column with the other existing notes.
- Clicking on an existing note in the list in the left-hand column should display that note in the right-hand column.
- Clicking on the Write icon in the navigation at the top of the page should display empty fields to enter a new note title and the note's text in the right-hand column.

## Installation

1. Clone the repository: git clone https://github.com/sunainaojha/note-taker
2. Navigate to the project directory: cd note-taker
3. Install the dependencies: npm install

## Technologies used
1. Node,js
2. Express.js
3. fs module
4. npm packages
5. HTML
6. CSS
7. JavaScript
8. JSON


## Usage

### Back-end

- The application includes a db.json file that is used to store and retrieve notes using the fs module.
- The following HTML routes are created:

  - GET /notes returns the notes.html file.
  - GET * returns the index.html file.

- The following API routes are created:

  - GET /api/notes reads the db.json file and returns all saved notes as JSON.
  - POST /api/notes receives a new note to save on the request body, adds it to the db.json file, and then returns the new note to the client.

- Each note is given a unique ID when saved, using an appropriate npm package.

- *Bonus*: The application also includes a DELETE route:

  - DELETE /api/notes/:id receives a query parameter that contains the ID of a note to delete.


  ## Links
[GitHub](https://github.com/sunainaojha/Note-taker)

[URL of Functional, deployed Application](https://pacific-coast-28426-1e5aac2b92fb.herokuapp.com/)

## Credits 
Suanina Ojha.