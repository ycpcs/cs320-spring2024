---
layout: default
title: "Lab02a: Web Applications II Lab Sign-Off"
---

Tests for Web Applications II Lab (Lab02a) Sign-Off
===============
 1) Pull up **Lab02a** in Eclipse: Verify that lab has been correctly refactored: **"lab02"** replaced with **"lab02a\_xxxx"**, where "xxxx" is the student's YCP username (look at the package names in Eclipse)

 2) Pull up the **Index page**: Verify that the URL contains **"lab02a\_xxxx"**, where "xxxx" is the student's YCP username

 3) Go to **Add Numbers** from the **Index page**: The **AddNumbers** page appears, with three number fields

 4) Enter **three numbers**: Get correct result
 
 5) Delete the **third number**: Get correct error message: **"Please enter 3 numbers"**, with all fields still filled with the submitted values
 
 6) Replace the **third number** with **"abc"**: Get correct error message: **"Invalid double"**, with all fields still filled with the submitted values

 7) Go back to the **Index Page**

 8) Go to **Multiply Numbers** from the **Index page**: The **MultiplyNumbers** page appears, with two number fields
 
 9) Enter **two numbers**: Get correct result
 
10) Delete the **first number**: Get correct error message: **"Please enter 2 numbers"**, with all fields still filled with the submitted values

11) Replace **first number** with **"abc"**: Get correct error message: **"Invalid double"**, with all fields still filled with the submitted values

12) Go back to the **Index Page**

13) Go to **Guessing Game** from the **Index page**: The **GuessingGame** page appears, with **"Start Game"** displayed

14) Use **33** as the number trying to be guessed: Press the correct buttons for each guess, eventually guesses 33
Correct sequence of guesses: **50** -> **25** -> **37** -> **31** -> **34** -> **32** -> **33**

15) Pull up **Numbers.java**: Verify that it exists

16) Pull up **addNumbers.JSP**: Verify that it is pulling data for the fields directly from the **Numbers.java** model, and **NOT** using values passed in as named parameters through the Servlet (except for the **Numbers.java** model reference)

17) Run test cases for **MultiplyNumbersController.java** controller and **Numbers.java** model: Test cases exist and pass