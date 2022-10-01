# api-auth-php-noframework-project
REST API PHP project with Udemy course, without framework, from scratch - https://www.udemy.com/course/create-a-rest-api-using-basic-php-with-token-authentication/</br>
# Strengths</br>
-Proper error handling, use of custom exceptions</br>
-Use of PDO for DB connection with bind parameters</br>
-Thinking ahead and keeping code clear, clean, separated properly - DB class returns write and read database. Can be improved in future</br>
-Response class and Task model are really well-written OOP in my opinion - Ive seen better php OOP, but not that often</br>
-Even though this is from-scratch pure PHP project, the author is very pedantic covering all sorts of problems and issues (status codes, charset, headers, cache and so on), there is this feeling author has thought of everything and I could really learn how such things work under the hood</br>
-You learn some additional skills that are not syntax or how to write code, but rather how HTTP, apache, API, auth, client server communication and many other thing work instead of relying on external libraries to magically do the stuff you dont understand - which is normally good, but such projects are good for learning</br>

# Weaknesses:</br>
-Does not use framework for API construction (thats the point of the project)</br>
-Does not use external libraries (thats the point of the project, but to be honest using .env for dsn elements wouldnt hurt) </br>
-In sessions.php a lot of repetitive code even though the whole project is well written, but still i think something could be done about it</br>
-I might not understand HTTP verbs fully, but I'm puzzled every time I have to use PATCH or PUT verbs... Why? Why not POST? The way i see it there is GET method that is default, does not have a body, can be used with query params to pass some information (potential security risk) or without them and there is POST method that is, the way i see it, not something alternative to GET but rather GET + POST body so every time you use POST you in a way use GET too. And you can even pass the information using BOTH POST body and GET query params. So these are the methods, thats how they act, but whats the difference between using POST and PUT, PATCH and so on? I mean, if api relies on using the same, identical route for different actions then maybe it makes sense... But still do I not understand if POST method and PUT/PATCH methods are any different from each other? This is thinking about things under the hood, but I would like to know how those methods work and surely will have to investigate (wireshark?).
