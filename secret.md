<h1>Secret</h1>

06ᵗʰ January 2023

Author: Axel Carachure


<h2>Description:</h2>

This challenge is about a conversation that was retrieved from a chat room via a social network.

<h2>Objective:</h2>

Find the secret text.

<h2>Difficulty:</h2>

Easy

<h2>Flag:</h2> 

HTB{StEnoGraPHy_TeXt}

<h1>Challenge</h1>

<h1>Solver</h1>

Hello, we are presented with a .zip file, called "chat.zip", let's start extracting this file with the following command: unzip chat.zip, the password is "hackthebox", we are shown a file called "chat.txt", when reading with cat we can see a normal chat which gives us confidential information, which tells us that the password of this chat is "password123". to know if the text uses stenography we can try to copy the same text and copy it in the console, if you see the following it means that the text is stenographed .

<img src="https://i.postimg.cc/JzQ6j2Hc/challenge-text.png" alt="Text">

We see something strange when copying this text, why not try the password that John indicated?.

We can use the following command to get the flag: stegcloak reveal -f chat.txt , indicating the password: "password123" or we can reveal each message (copying from the colon that separates the user and the message), this to see which of all the text uses stenography.

<img src="https://i.postimg.cc/BQpHp9N6/secret.png" alt="Secret"></img>
