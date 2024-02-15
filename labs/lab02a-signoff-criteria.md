---
layout: default
title: "Lab02a: Web Applications II Lab Sign-Off"
---

Tests for Web Applications II Lab (Lab02a) Sign-Off
===============
 1) Pull up **Lab02a** in Eclipse: Verify that the Project name has been changed to **"CS320\_lab02a\_username"**, where "username" is the student's YCP username.

 2) Pull up the **Index page**: Verify that the there are links/buttons for **AddNumbers**, **MultiplyNumbers**, and **GuessingGame**.

 3) Go to **Add Numbers** from the **Index page**: The **AddNumbers** page appears, with three number fields.

 4) Enter **three numbers**: Get correct sum.
 
 5) Delete the **third number**: Get correct error message: **"Please enter 3 numbers"** (required), with all fields still filled with the submitted values (optional extra credit).
 
 6) Replace the **third number** with **"abc"**: Get correct error message: **"Invalid double"** (required), with all fields still filled with the submitted values (optional extra credit).

 7) Go back to the **Index Page**.

 8) Go to **Multiply Numbers** from the **Index page**: The **MultiplyNumbers** page appears, with two number fields.
 
 9) Enter **two numbers**: Get correct product.
 
10) Delete the **first number**: Get correct error message: **"Please enter 2 numbers"** (required), with all fields still filled with the submitted values (optional extra credit).

11) Replace **first number** with **"abc"**: Get correct error message: **"Invalid double"** (required), with all fields still filled with the submitted values (optional extra credit).

12) Go back to the **Index Page**.

13) Go to **Guessing Game** from the **Index page**: The **GuessingGame** page appears, with **"Start Game"** displayed.

14) Use **33** as the number trying to be guessed: Press the correct buttons for each guess, application eventually guesses 33 on its own.  Correct sequence of guesses: **50** -> **25** -> **37** -> **31** -> **34** -> **32** -> **33**.

15) Pull up **Numbers.java**: Verify that it exists.

16) Pull up **addNumbersServlet.java**: Verify that it is **only** setting the **error message** and the **model** in the HTTP request before forwarding the HTTP request to the JSP.

17) Pull up **multiplyNumbers.JSP**: Verify that it is pulling data for the fields directly from the **Numbers.java** model, and **NOT** using values passed in as named parameters through the Servlet (except for **error message** and the **Numbers.java** model reference).

18) Run test cases for **NumbersController.java** controller and **Numbers.java** model: Test cases exist and pass.  A complete set of test cases should cover the **constructor(s)**, the **getters**, **setter(s)**, and the **add** and **multiply** methods.