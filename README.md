# Password-Hacker
You will learn how hacking works. You will work with iterators and generators, and you’ll learn a little something about the itertools module – one of the most powerful features of Python.
You will practice developing a client app and connecting to a server using the socket module. The project will also get you acquainted with JSON and the time module.

## Work on project. Stage 1/5: Establishing a connection
### Objectives
Your program will receive command line arguments in this order:

1. IP address
2. port
3. message for sending
The algorithm is the following:

1. Create a new socket.
2. Connect to a host and a port using the socket.
3. Send a message from the third command line argument to the host using the socket.
4. Receive the server’s response.
5. Print the server’s response.
6. Close the socket.

## Work on project. Stage 2/5: Simple brute force
### Objectives
In this stage, you should write a program that:

1. Parses the command line and gets two arguments that are IP address and port.
2. Tries different passwords until it finds the correct one.
3. Prints the password it found.
Note that you can connect to the server only once and then send messages many times. Don't connect to the server before sending every message.

Also, note that here and throughout the project, the password is different every time you check your code.

## Work on project. Stage 3/5: Smarter, dictionary-based brute force
### Objectives
In this stage, you should write a program that:

1. Parses the command line and gets two arguments that are IP address and port.
2. Finds the correct password using the list of typical passwords.
3. Prints the password it found.
Note that here and throughout the project, the password is different every time you check your code.

## Work on project. Stage 4/5: Catching exception
### Objectives
Your algorithm is the following:

1. Try all logins with an empty password.
2. When you find the login, try out every possible password of length 1.
3. When an exception occurs, you know that you found the first letter of the password.
4. Use the found login and the found letter to find the second letter of the password.
5. Repeat until you receive the ‘success’ message.
Finally, your program should print the combination of login and password in JSON format. 
The examples show two ways of what the output can look like. See the hint to find out how to convert a dict object into a JSON string.

## Work on project. Stage 5/5: Time-based vulnerability
### Objectives
In this stage, you should write a program that uses the time vulnerability to find the password.

- Use the list of logins from the previous stage.
- Output the result as you did this in the previous stage.
