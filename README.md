# SmartBrainBackEnd
Backend of SmartBrain project. 

Includes the Clarifai API used to detect a face in an image.
A database named 'smartbrain' which contains two tables in the schema, users and login.
where the users register information is stored and the password is encrypted and loaded into a seperate table (login)

The password encryption is handled by a bcrypt-nodejs plugin where the entered value is hashed and then referenced when user logs in.

The SmartBrainFrontEnd repo goes hand in hand with this repo. The front end utilizes REACT to compile your page and has tachyons in the js files to handle the look and style of the page.
First clone the repos, then run the backend and then the front end. 
Once registered/logged in you can copy an image url and past it into the input box. Hit detect and let Clarifai's API work its magic to draw a box around a face in your image. 
The more you detect the higher your score(entries) will be.
