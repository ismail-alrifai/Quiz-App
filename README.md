# Quiz-App
Questions With Choices.

For Run:
    
    1- Run "redis-server.exe" => The cache.
    
    2- In console "npm start" => Wait the database connection statement.

For Try The Routes:
    
    - Import the Postman Collection in the postman.

// --------------------------------------------------------------------- //

The quiz app contains:
    
    1- Admin Routes:
       which make admin able to add, update and delete a question also he can get all questions
       and get a specific question by id.

    2- Applicant Routes:
       he can get a randomized quiz questions by the type of questions (Backend, Frontend,... etc).
       also when he submit we take the answers and the questions ans compare it then get his score,
       if he succeed the frontend render a form to enter his information and when submit we save his
       info and send him an email using gmail automatically.

// --------------------------------------------------------------------- //

Notes:
   
   - The query of get all question is expensive and take time so i make it faster using caching.
      So when another applicant get a new quiz we will not make a database query instead we will
      return the questions immediately.

    - When applicant submit his answers we send a list of questions ids to avoid any try of cheating.
