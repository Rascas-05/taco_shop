# taco_shop
Taco Shop HTML challenge from Dave Gray HTML Full Course for Beginners - Complete All-in-One Tutorial - 4 Hours Feb 19 2022
VSCOde build notes for The Little Taco Shop HTML Challenge
----------------------------------------------------------
HTML Full Course for Beginners - Complete All-in-One Tutorial - 4 Hours Feb 19 2022
https://www.youtube.com/watch?v=mJgBOIoGihA
https://github.com/gitdagray/html_course

Prerequisites:
Windows 10 or later. 
I'm using Windows 10 Home with 32GB of memory on a Dell Dell Inspiron 5675
Any Laptop running Windows 10 or late will be fine for this project. 

Microsoft Visual Studio Code (VSCode)
If your a beginner new to VSCode, checkout VSCode beginner Tutorials on YouTube.


To follow along with my project build notes you may need to install some or all of the following VSCOde extensions as I will be taking advantage of AI assisted coding technologies:  
Note I have VSCOde Extensions installed that assists with HTML coding in VSCode:
GitHub Codespaces - GitHub
GitHub Copilot - GitHub
GitHubCopilot Chat - GitHub
GitHub Repositories - GitHub
Intellicode - Microsoft
Live Preview - Microsoft
Live Server - Ritwick Day
Open Folder Context Menus for VS Code - Chris Dias
Prettier - Code Formatter - Prettier
Remote Explorer - Microsoft
Remote Repositories - Microsoft
vscode-icons - VSCode Icons Team
Windows Terminal Integration - Daniel Imms

Also use "chatGPT4.com free" to help if you get stuck
https://openai.com/index/gpt-4o-and-more-tools-to-chatgpt-free/

Provided resources in 10_Lesson_Starter

Create a new public repository 'taco_shop' select README.md add About ->
"Taco Shop HTML challenge from Dave Gray HTML Full Course for Beginners - Complete All-in-One Tutorial - 4 Hours Feb 19 2022 
About"

Copy taco_shop repository link: https://github.com/Rascas-05/taco_shop.git

Open VSCOde in C:\Users\bfvdi\Documents\AppDevelopment\VSCODE\Projects\HTML

Open CMD Prompt Window cd C:\Users\bfvdi\Documents\AppDevelopment\VSCODE\Projects\HTML

C:\Users\bfvdi\Documents\AppDevelopment\VSCODE\Projects\HTML>code .<enter>

VSCOde opens in HTML folder.
Select "Clone Git Repository..." 
Select "Clone from Github ... remote sources 
Select "https://github.com/Rascas-05/taco_shop.git" 
Select Repository Destination "C:\Users\bfvdi\Documents\AppDevelopment\VSCODE\Projects\HTML"
Select "Open"
VSCode opens in "TACO_SHOP" folder with a README.md file.
--------------------------------------------------------------



Create a "templates' folder
Create a "css" folder under templates folder
Create a "html" folder under templates folder
Create a "img" folder
-----------------------
Use DOS CMD "tree /f /a" to provide a directory list.
Redirect the cmd output to a text file using "> tacoshoptree.txt" 
C:\Users\bfvdi\Documents\AppDevelopment\VSCODE\Projects\HTML\taco_shop>tree /f /a > tacoshoptree.txt
Folder PATH listing for volume OS
Volume serial number is 7AB7-27EC
C:.
|   README.md
|   tacoshoptree.txt
|   
+---img
\---templates
    +---css
    \---html
-----------------------------------
Copy image files provided by Dave Gray to "img" folder
Copy style.css file to templates\css folder
Copy 3 x web page designs to "img" folder  
- home-example.png
- hours-example.png
- contact-example.png
-----------------------------------
Folder PATH listing for volume OS
Volume serial number is 7AB7-27EC
C:.
|   README.md
|   tacoshoptree.txt
|   
+---img
|       contact-example.png
|       favicon.ico
|       home-example.png
|       hours-example.png
|       html5.png
|       tacos_and_drink_400x267.png
|       tacos_close_up_400x260.png
|       tacos_tray_400x267.png
|       
\---templates
    +---css
    |       style.css
    |       
    \---html
---------------------------------------
Create a new file "templates\html\index.html"
Open index.html file in VSCode editor
Type first line -> "!DOCTYPE "html"
Copilot will then prompt with suggested code. Press tab key to accept suggested code.
----index.html----
!DOCTYPE "html"
html
  head
    title= title
  body
    h1= title
    p Welcome to #{title}
------
Fix HTML code ->
Right click index.html in VSCode editor and select "Co-Pilot->Fix"
<!DOCTYPE html>
<html>
  <head>
    <title>Welcome to The Little Taco Shop</title>
  </head>
  <body>
    <h1>{{ title }}</h1>
    <p>Welcome to {{ title }}</p>
  </body>
</html>
---------
Edit title -> "Welcome to The Little Taco Shop"
View index.html with liveserver extension:
In VSCode click on "Go Live" located in bottom status line to the right to view your HTML file in Web browser.
Note. Liveserver will bitch if you don't have an acceptable minimal skeleton html file and shutdown the extension, and the "Go Live" link will not appear in the status bar. Close and reopen VSCOde and the "Go Live" link will reappear.
-----
Web Browser link/URL -> http://127.0.0.1:5500/templates/html/index.html
Note I used MS Paint to create LiveServer screenshots. 
C:\Users\bfvdi\Documents\AppDevelopment\VSCODE\Projects\HTML\taco_shop\img\LiveServer\index.html_minimal-skeleton.png
With reference to picture "home-example.png" start entering the text into a <body> section.
------
To hideVSCode Explorer panel -> clink on index.html file in (set focus to) editor panel then ->Ctrl+b
Resize VSCOde window vertically to half screen width.
Open home-example.png in MS Paint. Resize MS Paint window and position so that you can view both at the same time.
The two half windows shouldn't overlap
------
I typed out the following into VSCode editor:
---index.html---
<!DOCTYPE html>
<html>
  <head>
    <title="Welcome to The Little Taco Shop"></title>
  </head>
  <body>
    <section welcome>
    <h1>Welcome to The Little Taco Shop</h1>
    
    <--- link list bullet points -->
    <p>About LTS</p>
    <p>Our Nenu</p>
    <p>Store Hours</p>
    <p>Contact Us</p>
    <--- end Navigation list-->

    <--- link to Image of Tacos -->
    <p>Tacos and a Drink</p>
    </section>
    <hr>
        
    <Section about>
    <h2>About LTS</h2>
    <p>LTS was founded in 2022. Our shop was built from a love of tacos.
      <--- insert 3 taco emoji images --->. We hope our shop adds a unique and interesting place to our town.</p>

    <h3>Taco Trivia</h3>
    
    <--- Trivia drop down list --->
    <p>What is the most popular taco in the United States?</p>
    <p>What is the most popular taco in Mexico?</p>
    <p>When did tacos first appear in the United States?</p>
    <--- end trivia list --->

    </Section>
    <hr>

    <section menu>
    <h2>Our Menu</h2>
    <--- table 9 rows and 3 columns --->
    
    <--- end table --->

    <--- link Back_to_Top --->
    <p> Back_to_Top</p>
    <--- end link --->
    </section>

    <hr>
    <--- insert copyright symbol --->
    <P>Copyright The Litte Taco Shop</p>
    <--- --->
    
  </body>
</html>
-----index.html image in Live Server-----
index.html_filled-out-skeleton.png
=========================================
---------------------------------------------------------
Check text for typing errors errors.
Check alignment and postioning of web page elements.
View index.html and Live server side by side vertically.
Hide VSCode Explorer panel 
=========================================
My typing errors, alignment and postioning:
<p>Our Nenu</p> -> <p>Our Menu</p>
-----
Insert <br>
   <--- end Navigation list-->

    <br>

   <--- link to Image of Tacos -->
-----
Missing 'little'
We hope our shop adds a unique and interesting place to our town.</p>
We hope our shop adds a unique and interesting place to our little town.</p>
-----
==========================================
Fill in link list code for <section welcome>
----index.html - <section welcome> ----
    <--- link list bullet points -->
    <p>About LTS</p>
    <p>Our Menu</p>

    <--- Link hours.html --->
    <p>Store Hours</p>
    <--- Link contact.html --->
    <p>Contact Us</p>
    <--- end Navigation list-->


------
Add image link to <section welcome>
    <--- link to Image of Tacos -->
    <p>Tacos and a Drink</p>
    </section>
----------
In VSCode create the following files:
- "hours.html"
- "contact.html"
Add a minimal skeleton outline for each file
----home.html----
rename "index.html" as "home.html" 
-------
Add the following code to 'hours.html"
-------
<!DOCTYPE html>
<html>
  <head>
    <title>Welcome to The Little Taco Shop</title>
  </head>
  <body>
    <h1>{{ title }}</h1>
    <p>Welcome to {{ title }}</p>
  </body>
</html>
-----------------
create 'hours.html' skeleton outline using 'hours-example.png'
<!DOCTYPE html>
<html>
  <head>
    <title>Little Taco Shop Hours</title>
  </head>
  <body>
    <section hours>
    
    <--- page links --->

    <--- insert taco image --->

    <hr>

    <section hours </hours>
    <p>We are open 7 days a week!</p>

    <br>
    <h1>Little Taco Shop Hours</h1>

    <--- link back to top --->
    <lr>
     
    <--- Copyright -->
  </body>
</html>
----hours.html skeleton update ----
<!DOCTYPE html>
<html>
  <head>
    <title>Little Taco Shop Hours</title>
  </head>
  <body>
    <section hours>
    
    <--- page links --->

    <br>

    <--- insert taco image --->

    <hr>

    <section hours>
    <p>We are open 7 days a week!</p>

    <br>
    <h1>Little Taco Shop Hours</h1>

    <--- link back to top --->
    
    <br>
    
    <hr>

    <--- Copyright -->
  </body>
</html>
-----contact.html-skeleton ----------
create 'contact.html' skeleton outline using 'contact-example.png'
-------
<!DOCTYPE html>
<html>
  <head>
    <title>Contact Us</title>
  </head>
  <body>
    <section hours>
    
    <h1>Contact Us</h1>

    <--- page links --->

    <--- insert taco image --->

    <section contact form>
    
    <p>Our Contact Form</p>

    <--- wrap a frame around te form --->

    <--- insert contact form --->
    <br>

    <--- insert buttons ---> 
     <h1></h1>

    <--- link back to top --->
    <lr>
     
    <--- Copyright -->
  </body>
</html>
-----------------
img\liveserver\contact.html_skeleton.png
-----------------
Link hours.html and contact.html to home.html
---home.html-links---
<--- create href link to  templates\html\home.html --->
<--- create href link to templates\html\hours.html --->
<--- create href link to templates\html\contact.html --->

<--- create href link to  About LTS --->
<--- create href link to  Our Menu --->
<--- create href link to  Store Hours--->
<--- create href link to  Contact Us --->

<--- create href link to  templates\html\home.html --->
<--- create href link to templates\html\hours.html --->
<--- create href link to templates\html\contact.html --->
<--- create href link to templates\img\favicon.png --->
<--- resize image height=40 favicon.png --->
<--- create href link to templates\img\tacos_and_drink_400x267.png --->
<--- resize image height=400 width=267 tacos_and_drink_400x267.png --->
------- use chatGPT4 to create links
<a href="templates/html/home.html">Go to Home</a>
<a href="templates/html/hours.html">Hours</a>
<a href="templates/html/contact.html">Contact</a>
<a href="templates/img/favicon.png"></a>
<a href="templates/img/tacos_and_drink_400x267.png">
    <img src="templates/img/tacos_and_drink_400x267.png" alt="Tacos and Drink" height="400" width="267">
</a>
=======================
Section navigation fix: Query chatGPT4
"fix navigate to <section "welcome"> <a href="home.html">Back_to_Top</a>"
----------
To fix the HTML code for navigating to a section called "welcome" and create a link that goes back to the top, you can do the following:

1. Ensure that the `<section>` has an `id` that matches the link's target.
2. Use the correct syntax for the anchor link.

Here’s an updated version of your code:

```html
<section id="welcome">
    <!-- Your content here -->
</section>

<a href="#welcome">Back to Top</a>
```

In this example, the link will scroll back to the "welcome" section when clicked. If you want to link to the top of the page, you can use:

```html
<a href="#top">Back to Top</a>
```

And ensure there’s an element with the `id` of `top` at the top of your page:

```html
<div id="top"></div>
``` 

Let me know if you need any more help!
===========================================
---home.html---
Work on Trivia drop down list
query chatGPT4: "create html trivia drop down list"
---
Sure! Here’s a simple HTML code snippet for a trivia drop-down list. This example includes a few trivia questions with multiple-choice answers.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Trivia Drop-Down List</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
        }
        select {
            margin-bottom: 20px;
            padding: 10px;
        }
    </style>
</head>
<body>

    <h1>Trivia Quiz</h1>

    <label for="trivia-questions">Choose a trivia question:</label>
    <select id="trivia-questions">
        <option value="">Select a question</option>
        <option value="q1">What is the most popular taco in the United States?</option>
        <option value="q2">What is the most popular taco in Mexico?</option>
        <option value="q3">When did tacos first appear in the United States?</option>
    </select>

    <div id="answers" style="display: none;">
        <label for="answers">Select your answer:</label>
        <select id="answer-options">
            <option value="">Select an answer</option>
            <option value="a1">classic crunchy taco<</option>
            <option value="a2">taco al pastor</option>
            <option value="a3">Early 1900s</option>
        </select>
    </div>

    <script>
        const triviaSelect = document.getElementById('trivia-questions');
        const answersDiv = document.getElementById('answers');
        const answerOptions = document.getElementById('answer-options');

        triviaSelect.addEventListener('change', function() {
            if (this.value) {
                answersDiv.style.display = 'block';
                // Clear previous options
                answerOptions.selectedIndex = 0;

                // Change answer options based on the selected question
                if (this.value === 'q1') {
                    answerOptions.innerHTML = `
                        <option value="">Select an answer</option>
                        <option value="a1">beef taco</option>
                        <option value="a2">classic crunchy taco</option>
                        <option value="a3">breakfast tacos</option>
                    `;
                } else if (this.value === 'q2') {
                    answerOptions.innerHTML = `
                        <option value="">Select an answer</option>
                        <option value="a1">taco al pastor</option>
                        <option value="a2">tacos de barbacoa</option>
                        <option value="a3">tacos de pollo</option>
                    `;
                } else if (this.value === 'q3') {
                    answerOptions.innerHTML = `
                        <option value="">Select an answer</option>
                        <option value="a1">Early 1800s</option>
                        <option value="a2">Late 1800s</option>
                        <option value="a3">Early 1900s</option>
                    `;
                }
            } else {
                answersDiv.style.display = 'none';
            }
        });
    </script>

</body>
</html>
```

### Explanation:
- **HTML Structure**: A drop-down list for trivia questions and another one for answers.
- **JavaScript**: Listens for changes in the trivia question selection. When a question is selected, the answer options update accordingly.
- **Styling**: Basic styling to make it look clean.

Feel free to modify the questions and answers as needed! 
------
<html lang="en">
add to existing <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Trivia Drop-Down List</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
        }
        select {
            margin-bottom: 20px;
            padding: 10px;
        }
    </style>
-------
Edit trivia questions & answers
----
<body>

    <h1>Trivia Quiz</h1>

    <label for="trivia-questions">Choose a trivia question:</label>
    <select id="trivia-questions">
        <option value="">Select a question</option>
        <option value="q1">What is the capital of France?</option>
        <option value="q2">Who wrote 'Romeo and Juliet'?</option>
        <option value="q3">What is the largest planet in our Solar System?</option>
    </select>

    <div id="answers" style="display: none;">
        <label for="answers">Select your answer:</label>
        <select id="answer-options">
            <option value="">Select an answer</option>
            <option value="a1">Paris</option>
            <option value="a2">Rome</option>
            <option value="a3">London</option>
        </select>
    </div>

    <script>
        const triviaSelect = document.getElementById('trivia-questions');
        const answersDiv = document.getElementById('answers');
        const answerOptions = document.getElementById('answer-options');

        triviaSelect.addEventListener('change', function() {
            if (this.value) {
                answersDiv.style.display = 'block';
                // Clear previous options
                answerOptions.selectedIndex = 0;

                // Change answer options based on the selected question
                if (this.value === 'q1') {
                    answerOptions.innerHTML = `
                        <option value="">Select an answer</option>
                        <option value="a1">Paris</option>
                        <option value="a2">Rome</option>
                        <option value="a3">London</option>
                    `;
                } else if (this.value === 'q2') {
                    answerOptions.innerHTML = `
                        <option value="">Select an answer</option>
                        <option value="a1">William Shakespeare</option>
                        <option value="a2">Charles Dickens</option>
                        <option value="a3">Mark Twain</option>
                    `;
                } else if (this.value === 'q3') {
                    answerOptions.innerHTML = `
                        <option value="">Select an answer</option>
                        <option value="a1">Earth</option>
                        <option value="a2">Jupiter</option>
                        <option value="a3">Saturn</option>
                    `;
                }
            } else {
                answersDiv.style.display = 'none';
            }
        });
    </script>

</body>
--------
Revised the query chatGPT4: "fix code to display submit button when a trivia question answer has been selected and display if the answer is corrent or not 'and appended the previous trivia code"
-----
Here’s a revised version of your code that ensures the submit button only displays when an answer is selected and provides feedback on whether the answer is correct or not. I've fixed some issues in your original code and organized it for clarity:

```html
<!-- Trivia drop down list -->
<label for="trivia-questions">Choose a trivia question:</label>
<br>
<select id="trivia-questions">
    <option value="">Select a question</option>
    <option value="q1">What is the most popular taco in the United States?</option>
    <option value="q2">What is the most popular taco in Mexico?</option>
    <option value="q3">When did tacos first appear in the United States?</option>
</select>

<div id="answers" style="display: none;">
    <label for="answer-options">Select your answer:</label>
    <select id="answer-options">
        <option value="">Select an answer</option>
    </select>
</div>

<!-- Add trivia answer button -->
<button id="trivia-answer" style="display: none;">Submit Answer</button>
<br>

<!-- Get trivia question response -->
<p id="trivia-response"></p>

<script>
    const triviaSelect = document.getElementById('trivia-questions');
    const answersDiv = document.getElementById('answers');
    const answerOptions = document.getElementById('answer-options');
    const triviaResponse = document.getElementById('trivia-response');
    const triviaAnswer = document.getElementById('trivia-answer');

    triviaSelect.addEventListener('change', function() {
        if (this.value) {
            answersDiv.style.display = 'block';
            triviaAnswer.style.display = 'none'; // Hide button initially
            answerOptions.selectedIndex = 0;

            // Change answer options based on the selected question
            if (this.value === 'q1') {
                answerOptions.innerHTML = `
                    <option value="">Select an answer</option>
                    <option value="a1">beef taco</option>
                    <option value="a2">classic crunchy taco</option>
                    <option value="a3">breakfast tacos</option>
                `;
            } else if (this.value === 'q2') {
                answerOptions.innerHTML = `
                    <option value="">Select an answer</option>
                    <option value="a1">taco al pastor</option>
                    <option value="a2">tacos de barbacoa</option>
                    <option value="a3">tacos de pollo</option>
                `;
            } else if (this.value === 'q3') {
                answerOptions.innerHTML = `
                    <option value="">Select an answer</option>
                    <option value="a1">Early 1800s</option>
                    <option value="a2">Late 1800s</option>
                    <option value="a3">Early 1900s</option>
                `;
            }
        } else {
            answersDiv.style.display = 'none';
            triviaResponse.textContent = '';
            triviaAnswer.style.display = 'none'; // Hide button
        }
    });

    answerOptions.addEventListener('change', function() {
        if (this.value) {
            triviaAnswer.style.display = 'block'; // Show button
            // Check for correct answers based on selected question
            if ((triviaSelect.value === 'q1' && this.value === 'a2') || 
                (triviaSelect.value === 'q2' && this.value === 'a1') || 
                (triviaSelect.value === 'q3' && this.value === 'a3')) {
                triviaResponse.textContent = 'Correct!';
            } else {
                triviaResponse.textContent = 'Incorrect, try again.';
            }
        } else {
            triviaResponse.textContent = '';
            triviaAnswer.style.display = 'none'; // Hide button
        }
    });

    triviaAnswer.addEventListener('click', function() {
        const selectedAnswer = answerOptions.value;
        if (selectedAnswer) {
            alert(triviaResponse.textContent);
        } else {
            alert('Please select an answer.');
        }
    });
</script>
<!-- end trivia list -->
```

### Key Changes:
1. **Button Visibility**: The submit button is hidden until an answer is selected.
2. **Feedback Display**: The trivia response now provides correct or incorrect feedback based on the selected answer.
3. **Code Organization**: Cleaned up event listeners to ensure they function as intended and avoid redundancy.

This code will properly display the submit button when an answer is selected and give feedback based on the user's selection.
-----
This new trivia code works fine!
======
Note commenting out this button breaks the script functioning correctly. 
<!-- Add trivia answer button -->
<button id="trivia-answer" style="display: none;">Submit Answer</button>
<br>
====================================
------home.html--work on menu table----
Compose chatGPT4 query: create html table 
row 1, no columns, Our Tacos 
row 2, 3 colums, Tacos, Qty, Price
row 4, 3 colums, Crunchy, 1, $1.50
row 4, 3 colums, Crunchy, 2, $2.50
row 5, 3 colums, Crunchy, 3, $3.25
row 6, 3 colums, Soft, 1, $2.00 
row 7, 3 colums, Soft, 2, $3.50
row 8, 3 colums, Soft, 3, $4.50
row 9, no columns, Chips, & Salsa $2
-----ChatGPT4 response-----
Here's the HTML code for the table you described:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Our Tacos</title>
    <style>
        table {
            width: 50%;
            border-collapse: collapse;
            margin: 20px auto;
        }
        th, td {
            border: 1px solid #000;
            padding: 8px;
            text-align: center;
        }
        th {
            background-color: #f2f2f2;
        }
        .no-border {
            border: none;
        }
    </style>
</head>
<body>

    <table>
        <tr>
            <td class="no-border" colspan="3"><strong>Our Tacos</strong></td>
        </tr>
        <tr>
            <th>Tacos</th>
            <th>Qty</th>
            <th>Price</th>
        </tr>
        <tr>
            <td>Crunchy</td>
            <td>1</td>
            <td>$1.50</td>
        </tr>
        <tr>
            <td>Crunchy</td>
            <td>2</td>
            <td>$2.50</td>
        </tr>
        <tr>
            <td>Crunchy</td>
            <td>3</td>
            <td>$3.25</td>
        </tr>
        <tr>
            <td>Soft</td>
            <td>1</td>
            <td>$2.00</td>
        </tr>
        <tr>
            <td>Soft</td>
            <td>2</td>
            <td>$3.50</td>
        </tr>
        <tr>
            <td>Soft</td>
            <td>3</td>
            <td>$4.50</td>
        </tr>
        <tr>
            <td class="no-border" colspan="3">Chips & Salsa $2</td>
        </tr>
    </table>

</body>
</html>
```

You can copy and paste this code into an HTML file, and it will display the table as you specified. Let me know if you need any modifications!
----
chatGPT4 table query response TACO_Shop\img\liverserver\our_mnu_table_query.png
-------
Fix table border top & bottom rows:
<td class="no-border" colspan="3"><strong>Our Tacos</strong></td>
changed to:
<td class="border" colspan="3"><strong>Our Tacos</strong></td>
---
<td class="no-border" colspan="3">Chips & Salsa $2</td>
changed to:
<td class="border" colspan="3">Chips & Salsa $2</td>
----
Fix Copyright symbol <P>Copyright The Litte Taco Shop</p>
To include a proper copyright symbol in your HTML, you can use the HTML entity `&copy;`. Here’s how to fix your paragraph:

```html
<p>&copy; The Little Taco Shop</p>
```

Make sure to use the correct spelling of "Little" as well. If you want the paragraph to have a specific style or alignment, you can add some CSS too. Let me know if you need help with that!
-----
Fix Home page link order and names (top)
About LTS
Our Menu
Store Hours
Contact Us
----
Add bullet points to left of link names.
----
chatgPT4 query: "add bullet html list About LTS
Our Menu
Store Hours
Contact Us"
---
You can create a bullet list in HTML using the `<ul>` (unordered list) and `<li>` (list item) tags. Here’s how to add that list for "About LTS," "Our Menu," "Store Hours," and "Contact Us":

```html
<h2>About LTS</h2>
<ul>
    <li>Our Menu</li>
    <li>Store Hours</li>
    <li>Contact Us</li>
</ul>
```

You can place this code anywhere in your HTML document where you want the list to appear. Let me know if you need further assistance!
----
</ul>
  <li><a href="about.html">About LTS</a><li>
  <br>
  <li><a href="menu.html">Our Menu</a><li>
  <br>
  <li><a href="hours.html">Store Hours</a><li>
  <br>
  <li><a href="contact.html">Contact Us</a><li>
</ul>
<br>
----
Links don't work chatGPT4 ->
It looks like the closing tags for your list items are incorrect. You should use `</li>` instead of `<li>` at the end of each item. Here’s the corrected code:

```html
<ul>
    <li><a href="about.html">About LTS</a></li>
    <li><a href="menu.html">Our Menu</a></li>
    <li><a href="hours.html">Store Hours</a></li>
    <li><a href="contact.html">Contact Us</a></li>
</ul>
```

This will properly create a list of links. Let me know if you need any more help!
To print a bullet point symbol in HTML, you can use the HTML entity `&bull;`. Here’s how you can display it:

```html
<p>&bull;</p>
```

If you want to use it in a list format, you can do something like this:

```html
<ul>
    <li>&bull; Item 1</li>
    <li>&bull; Item 2</li>
    <li>&bull; Item 3</li>
</ul>
```
This will show bullet points before each item. Let me know if you need anything else!
---
</ul>
  <li>&bull;<a href="about.html">About LTS</a><li>
  <li>&bull;<a href="menu.html">Our Menu</a><li>
  <li>&bull;<a href="hours.html">Store Hours</a><li>
  <li>&bull;<a href="contact.html">Contact Us</a><li>
</ul>
----
Try this:
   &bull;<a href="about.html">About LTS</a> 
   &bull;<a href="menu.html">Our Menu</a> 
   &bull;<a href="hours.html">Store Hours</a> 
   &bull;<a href="contact.html">Contact Us</a> 
-----
To insert a space after the bullet point symbol (`&bull;`), you can simply add a non-breaking space (`&nbsp;`) or a regular space after it. Here’s how you can do it:

```html
<ul>
    <li>&bull;&nbsp;Item 1</li>
    <li>&bull;&nbsp;Item 2</li>
    <li>&bull;&nbsp;Item 3</li>
</ul>
```

This will create a space after each bullet point. Let me know if you need further assistance!
----
I need to ackknowledge emoji source on web page.
<a href="https://www.freepik.com/search">Icon by tulpahn</a>

taco_2061199_512_512.png
----
Asked chatGPT4 to fix hours.html
Here's a corrected version of your HTML code with some improvements:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Little Taco Shop Hours</title>
    <style>
        body {
            font-family: Arial, sans-serif;
        }
        #hours {
            margin: 20px;
        }
        img {
            max-width: 100%; /* Ensure image is responsive */
            height: auto;
        }
    </style>
</head>
<body>
    <section id="hours">
        &bull;&nbsp;&nbsp;<a href="home.html">Home</a>
        <br>
        &bull;&nbsp;&nbsp;<a href="about.html">About LTS</a>
        <br>
        &bull;&nbsp;&nbsp;<a href="menu.html">Our Menu</a>
        <br>
        &bull;&nbsp;&nbsp;<a href="contact.html">Contact Us</a>
        <br><br>
        <a href="/img/tacos_tray_400x267.png">
            <img src="/img/tacos_tray_400x267.jpg" alt="Tray of Tasty Tacos" height="400" width="267">
        </a>
        <br>
        <p>A Tray of Tasty Tacos</p>
        <hr>
        <h2>We are open 7 days a week!</h2>
        <h3>Monday - Thursday</h3>
        <p>11am - 9pm</p>
        <h3>Friday - Saturday</h3>
        <p>11am - 11pm</p>
        <br>
        <a href="#hours">Back to Top</a>
        <hr>
        <p>&copy; The Little Taco Shop</p>
    </section>
</body>
</html>
```

### Key Fixes and Improvements:
1. **Corrected Links**: Fixed the `href` attributes in the "About" and "Our Menu" links. The previous format was incorrect.
2. **Meta Tags**: Added character set and viewport meta tags for better compatibility and responsiveness.
3. **CSS Styles**: Added basic styling to improve the layout and responsiveness.
4. **Alt Attribute**: Added an `alt` attribute to the image for better accessibility.
5. **Section Tag**: Removed the invalid `section hours` tag, as it was not used correctly.
6. **Text Formatting**: Simplified the display of operating hours for better clarity. 

Feel free to adjust the styles or content as needed!
----hours.html----
<a href="/img/tacos_tray_400x267.png">
<img src="/img/tacos_tray_400x267.jpg" alt="Tray of Tasty Tacos" height="400" width="267">
        </a>
Changed <img src="/img/tacos_tray_400x267.jpg"
file type to .png: (tacos_tray_400x267.png) 
Image now displays correctly.
----contact.html----
Our Location:
555 Taco Temptation Lane, Suite T
Kansas City, MO 55555-5555

Phone: 555-555-5555
----Contact form----

Create contact form:
frame wraps around
Name: your name

Email: your email

Your Message
Message edit box
Type your message here (Faint text)

Frame width - full page 
Frame height - half page width

Send button, Reset button

"Send Us a Message" place top left of frame

-------chatGPT4 query response----
Here's a simple HTML contact form with the specifications you provided. This form includes a frame that wraps around it, a message edit box with placeholder text, and buttons for sending and resetting the form.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Form</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }
        .contact-frame {
            width: 100%;
            height: 50vh;
            border: 1px solid #ccc;
            padding: 20px;
            box-sizing: border-box;
            position: relative;
        }
        h2 {
            position: absolute;
            top: 10px;
            left: 20px;
        }
        input[type="text"],
        input[type="email"],
        textarea {
            width: calc(100% - 40px);
            margin: 10px 0;
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        textarea {
            height: 100px;
            resize: none;
        }
        button {
            margin: 10px 5px;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .send-button {
            background-color: #4CAF50;
            color: white;
        }
        .reset-button {
            background-color: #f44336;
            color: white;
        }
    </style>
</head>
<body>

<div class="contact-frame">
    <h2>Send Us a Message</h2>
    <form>
        <label for="name">Name:</label>
        <input type="text" id="name" name="name" required>

        <label for="email">Email:</label>
        <input type="email" id="email" name="email" required>

        <label for="message">Your Message:</label>
        <textarea id="message" name="message" placeholder="Type your message here..." required></textarea>

        <button type="submit" class="send-button">Send</button>
        <button type="reset" class="reset-button">Reset</button>
    </form>
</div>

</body>
</html>
```

### Explanation:
- The form is wrapped in a `<div>` with the class `contact-frame`, which sets its width to 100% and height to half the viewport height (50vh).
- The form elements include a name input, an email input, and a textarea for the message, with appropriate labels.
- The buttons for sending and resetting the form are styled with different colors.
- The title "Send Us a Message" is positioned at the top left of the frame. 

You can copy and paste this code into an HTML file to see the form in action!
------
The following messages are display at the top of the form. probably due to css

<h2>Little Tacos Shop Tacos</h2>
<h2>Our Contact Form</h2>
<h2>Send Us a Message</h2>
------
Query chatGPT4 to "fix h2 titles showing top of page + paste all the code in contact.html
To fix the issue with the `<h2>` titles showing at the top of the page due to the absolute positioning, you can modify the CSS for the `<h2>` elements. Here’s a cleaned-up version of your HTML and CSS that ensures the titles are positioned correctly within their respective sections. 

### Updated Code

```html
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Us</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }
        #hours {
            margin: 20px;
        }
        img {
            max-width: 100%; /* Ensure image is responsive */
            height: auto;
        }
      
        .contact-frame {
            width: 100%;
            height: 50vh;
            border: 1px solid #ccc;
            padding: 20px;
            box-sizing: border-box;
            position: relative;
        }
        h1, h2 {
            margin: 20px 0; /* Add margin for spacing */
        }
        input[type="text"],
        input[type="email"],
        textarea {
            width: calc(100% - 40px);
            margin: 10px 0;
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        textarea {
            height: 100px;
            resize: none;
        }
        button {
            margin: 10px 5px;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .send-button {
            background-color: #4CAF50;
            color: white;
        }
        .reset-button {
            background-color: #f44336;
            color: white;
        }
    </style>
</head>
<body>
    <section id="hours">
        <h1>Contact Us</h1>
        &bull;&nbsp;&nbsp;<a href="home.html">Home</a><br>
        &bull;&nbsp;&nbsp;<a href="home.html#about">About LTS</a><br>
        &bull;&nbsp;&nbsp;<a href="home.html#menu">Our Menu</a><br>
        &bull;&nbsp;&nbsp;<a href="hours.html">Store Hours</a><br>
    </section>
    
    <br>
    <a href="/img/tacos_close_up_400x260.png">
        <img src="/img/tacos_close_up_400x260.png" height="400">
    </a>
    <br><br><br>
    
    <h2>Little Tacos Shop Tacos</h2>

    <section id="contact-form">
        <h2>Our Contact Form</h2>
        <h2>Send Us a Message</h2>
        <div class="contact-frame">
            <form>
                <label for="name">Name:</label>
                <input type="text" id="name" name="name" placeholder="Type your name here..." required>

                <label for="email">Email:</label>
                <input type="email" id="email" name="email" placeholder="Type your email here..." required>
                
                <label for="message">Your Message:</label>
                <textarea id="message" name="message" placeholder="Type your message here..." required></textarea>

                <button type="submit" class="send-button">Send</button>
                <button type="reset" class="reset-button">Reset</button>
            </form>
        </div>
    </section>

    <section id="location">
        <h2>Our Location</h2>
        <p>555 Taco Temptation Lane, Suite T</p>
        <p>Kansas City, MO 55555-5555</p>
        <p>Phone: 555-555-5555</p>
    </section>
    
    <hr> 
    <a href="#contact">Back to Top</a>
    <p>&copy; The Little Taco Shop</p>
</body>
</html>
```

### Key Changes
1. **Removed Absolute Positioning**: The `position: absolute` style from the `<h2>` elements was removed to allow them to flow naturally within the document structure.
2. **Margin for Titles**: Added margins to `<h1>` and `<h2>` elements for spacing.
3. **Corrected Links**: Fixed the `href` attributes for the "About LTS" and "Our Menu" links to ensure they work properly.

These adjustments will make the titles display correctly without being pushed to the top of the page.
-----
The new code fixed the the positing of the <h2> titles.
-----
resize width of name, email and message text input boxes to say 1/3 the width of the form.
---contact.html---
css
change "width: calc(100% - 40px);
to: "width: calc(33% - 40px);"
        input[type="text"],
        input[type="email"],
        textarea {
            width: calc(100% - 40px);
            margin: 10px 0;
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
----------
adjusting width % worked however the alignment of email and your message box changed.
ask chatGPT4 to change width of name, email and message boxes to 33% and retain vertical alignment of each element.
----
To change the width of the name, email, and message boxes to 33% while retaining their vertical alignment, you can modify the CSS for the input and textarea elements. Here’s the updated code:

```html
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Us</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }
        #hours {
            margin: 20px;
        }
        img {
            max-width: 100%; /* Ensure image is responsive */
            height: auto;
        }

        .contact-frame {
            width: 100%;
            height: 50vh;
            border: 1px solid #ccc;
            padding: 20px;
            box-sizing: border-box;
            position: relative;
        }
        h1, h2 {
            margin: 20px 0; /* Add margin for spacing */
        }
        label {
            display: block; /* Ensure labels take full width */
            margin: 10px 0 5px; /* Add margin for spacing */
        }
        input[type="text"],
        input[type="email"],
        textarea {
            width: 33%; /* Set width to 33% */
            margin: 10px 0;
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
            display: block; /* Ensure inputs and textarea are block-level elements */
        }
        textarea {
            height: 100px;
            resize: none;
        }
        button {
            margin: 10px 5px;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .send-button {
            background-color: #4CAF50;
            color: white;
        }
        .reset-button {
            background-color: #f44336;
            color: white;
        }
    </style>
</head>
<body>
    <section id="hours">
        <h1>Contact Us</h1>
        &bull;&nbsp;&nbsp;<a href="home.html">Home</a><br>
        &bull;&nbsp;&nbsp;<a href="home.html#about">About LTS</a><br>
        &bull;&nbsp;&nbsp;<a href="home.html#menu">Our Menu</a><br>
        &bull;&nbsp;&nbsp;<a href="hours.html">Store Hours</a><br>
    </section>
    
    <br>
    <a href="/img/tacos_close_up_400x260.png">
        <img src="/img/tacos_close_up_400x260.png" height="400">
    </a>
    <br><br><br>
    
    <h2>Little Tacos Shop Tacos</h2>

    <section id="contact-form">
        <h2>Our Contact Form</h2>
        <h2>Send Us a Message</h2>
        <div class="contact-frame">
            <form>
                <label for="name">Name:</label>
                <input type="text" id="name" name="name" placeholder="Type your name here..." required>

                <label for="email">Email:</label>
                <input type="email" id="email" name="email" placeholder="Type your email here..." required>
                
                <label for="message">Your Message:</label>
                <textarea id="message" name="message" placeholder="Type your message here..." required></textarea>

                <button type="submit" class="send-button">Send</button>
                <button type="reset" class="reset-button">Reset</button>
            </form>
        </div>
    </section>

    <section id="location">
        <h2>Our Location</h2>
        <p>555 Taco Temptation Lane, Suite T</p>
        <p>Kansas City, MO 55555-5555</p>
        <p>Phone: 555-555-5555</p>
    </section>
    
    <hr> 
    <a href="#contact">Back to Top</a>
    <p>&copy; The Little Taco Shop</p>
</body>
</html>
```

### Changes Made:
1. **Width Adjustment**: The width of the `input[type="text"]`, `input[type="email"]`, and `textarea` has been set to `33%`.
2. **Block Display**: Ensured that labels, inputs, and textareas are block-level elements to maintain vertical alignment. This allows each element to stack vertically and respect the specified widths. 

With these changes, the name, email, and message boxes will be 33% wide and maintain their vertical alignment in the form.
---
ask chatGPT4 to "indent left page margin 50 pixels paste full page code.
-----contact.html----
To indent the left page margin by 50 pixels, you can simply add a `padding-left` property to the `body` element in your CSS. Here’s the updated code:

```html
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Us</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            padding-left: 50px; /* Indent left margin by 50 pixels */
        }
        #hours {
            margin: 20px;
        }
        img {
            max-width: 100%; /* Ensure image is responsive */
            height: auto;
        }

        .contact-frame {
            width: 100%;
            height: 50vh;
            border: 1px solid #ccc;
            padding: 20px;
            box-sizing: border-box;
            position: relative;
        }
        h1, h2 {
            margin: 20px 0; /* Add margin for spacing */
        }
        label {
            display: block; /* Ensure labels take full width */
            margin: 10px 0 5px; /* Add margin for spacing */
        }
        input[type="text"],
        input[type="email"],
        textarea {
            width: 33%; /* Set width to 33% */
            margin: 10px 0;
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
            display: block; /* Ensure inputs and textarea are block-level elements */
        }
        textarea {
            height: 100px;
            resize: none;
        }
        button {
            margin: 10px 5px;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .send-button {
            background-color: #4CAF50;
            color: white;
        }
        .reset-button {
            background-color: #f44336;
            color: white;
        }
    </style>
</head>
<body>
    <section id="hours">
        <h1>Contact Us</h1>
        &bull;&nbsp;&nbsp;<a href="home.html">Home</a><br>
        &bull;&nbsp;&nbsp;<a href="home.html#about">About LTS</a><br>
        &bull;&nbsp;&nbsp;<a href="home.html#menu">Our Menu</a><br>
        &bull;&nbsp;&nbsp;<a href="hours.html">Store Hours</a><br>
    </section>
    
    <br>
    <a href="/img/tacos_close_up_400x260.png">
        <img src="/img/tacos_close_up_400x260.png" height="400">
    </a>
    <br><br><br>
    
    <h2>Little Tacos Shop Tacos</h2>

    <section id="contact-form">
        <h2>Our Contact Form</h2>
        <h2>Send Us a Message</h2>
        <div class="contact-frame">
            <form>
                <label for="name">Name:</label>
                <input type="text" id="name" name="name" placeholder="Type your name here..." required>

                <label for="email">Email:</label>
                <input type="email" id="email" name="email" placeholder="Type your email here..." required>
                
                <label for="message">Your Message:</label>
                <textarea id="message" name="message" placeholder="Type your message here..." required></textarea>

                <button type="submit" class="send-button">Send</button>
                <button type="reset" class="reset-button">Reset</button>
            </form>
        </div>
    </section>

    <section id="location">
        <h2>Our Location</h2>
        <p>555 Taco Temptation Lane, Suite T</p>
        <p>Kansas City, MO 55555-5555</p>
        <p>Phone: 555-555-5555</p>
    </section>
    
    <hr> 
    <a href="#contact">Back to Top</a>
    <p>&copy; The Little Taco Shop</p>
</body>
</html>
```

### Changes Made:
- **Left Margin Indentation**: Added `padding-left: 50px;` to the `body` CSS rule to create a left indentation of 50 pixels.

This adjustment will ensure all content is indented appropriately from the left side of the page.
-----
Reduced padding to 20px:
---

Adding padding for right margin
padding-right: 50px; /* Indent right margin by 50 pixels */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            padding-left: 20px; /* Indent left margin by 50 pixels */
            padding-right: 20px; /* Indent right margin by 50 pixels */
        }
----------
ask chatGPT4: 
fix phone number to link to phone dialler <p>Phone: 555-555-5555</p>
----
To make the phone number a clickable link that opens the phone dialer, you can use the `<a>` tag with the `tel:` protocol. Here’s how to modify the phone number in your code:

```html
<p>Phone: <a href="tel:5555555555">555-555-5555</a></p>
```

### Updated Section:
Here’s the complete relevant section of your HTML:

```html
<section id="location">
    <h2>Our Location</h2>
    <p>555 Taco Temptation Lane, Suite T</p>
    <p>Kansas City, MO 55555-5555</p>
    <p>Phone: <a href="tel:5555555555">555-555-5555</a></p>
</section>
```

### Explanation:
- The `href="tel:5555555555"` attribute specifies that this link should initiate a phone call when clicked.
- The number is formatted without dashes or spaces in the `tel:` link to ensure compatibility across devices.

With this change, users on mobile devices can click the phone number to start a call directly.
-----
Ask chatGPT to:
change the following text to italic:         
        <p>555 Taco Temptation Lane, Suite T</p>
        <p>Kansas City, MO 55555-5555</p>
        <p>Phone: 555-555-5555</p>
        <p>Phone: <a href="tel:5555555555">555-555-5555</a></p>
--------
To change the text to italic, you can wrap each `<p>` tag's content in `<em>` tags or use the `<i>` tag. Here’s how to modify your HTML:

```html
<section id="location">
    <h2>Our Location</h2>
    <p><em>555 Taco Temptation Lane, Suite T</em></p>
    <p><em>Kansas City, MO 55555-5555</em></p>
    <p><em>Phone: 555-555-5555</em></p>
    <p><em>Phone: <a href="tel:5555555555">555-555-5555</a></em></p>
</section>
```

### Explanation:
- Each line of text is now wrapped in `<em>` tags, which will render the text in italics. 

This change will ensure that all specified text appears italicized in the rendered output.
----
Text style fixed.
----
Ask chatGPT4 to:
position "<h5>Send Us a Message</h5>" as a part of the submit order form border, top left 
------
To position the <h5>Send Us a Message</h5> heading as part of the submit order form border in the top left corner, you can use CSS to style it and adjust its position. Here's how to do it:

Wrap the heading in the same container as the form.
Use absolute positioning for the heading.
Here's how you can modify the relevant section of your HTML:

<section id="contact-form">
    <h2>Our Contact Form</h2>
    <div class="contact-frame">
        <h5 style="position: absolute; top: 10px; left: 10px; margin: 0;">Send Us a Message</h5>
        <form>
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" placeholder="Type your name here..." required>

            <label for="email">Email:</label>
            <input type="email" id="email" name="email" placeholder="Type your email here..." required>
            
            <label for="message">Your Message:</label>
            <textarea id="message" name="message" placeholder="Type your message here..." required></textarea>

            <button type="submit" class="send-button">Send</button>
            <button type="reset" class="reset-button">Reset</button>
        </form>
    </div>
</section>
-----
CSS Considerations
You might also want to ensure the .contact-frame has position: relative; so that the absolutely positioned heading will be placed correctly within its context:
.contact-frame {
    width: 100%;
    height: 50vh;
    border: 1px solid #ccc;
    padding: 20px;
    box-sizing: border-box;
    position: relative; /* Ensure this is set for absolute positioning to work */
}
Explanation:
Positioning: The <h5> is positioned absolutely within the .contact-frame, which allows it to be placed at the top left corner (10 pixels from the top and left).
Margin: The margin is set to 0 to avoid any default spacing that could affect its position.
With these changes, the heading will appear neatly in the top left corner of the contact form's border.
----contact.html---
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Us</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            padding-left: 20px; /* Indent left margin by 50 pixels */
            padding-right: 20px; /* Indent right margin by 50 pixels */
        }
        #hours {
            margin: 20px;
        }
        img {
            max-width: 100%; /* Ensure image is responsive */
            height: auto;
        }

        .contact-frame {
        width: 100%;
        height: 50vh;
        border: 1px solid #ccc;
        padding: 20px;
        box-sizing: border-box;
        position: relative; /* Ensure this is set for absolute positioning to work */
        }
        h1, h2 {
            margin: 20px 0; /* Add margin for spacing */
        }
        label {
            display: block; /* Ensure labels take full width */
            margin: 10px 0 5px; /* Add margin for spacing */
        }
        input[type="text"],
        input[type="email"],
        textarea {
            width: 33%; /* Set width to 33% */
            margin: 10px 0;
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
            display: block; /* Ensure inputs and textarea are block-level elements */
        }
        textarea {
            height: 100px;
            resize: none;
        }
        button {
            margin: 10px 5px;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .send-button {
            background-color: #4CAF50;
            color: white;
        }
        .reset-button {
            background-color: #f44336;
            color: white;
        }
    </style>
</head>
<body>
    <section id="hours">
        <h1>Contact Us</h1>
        &bull;&nbsp;&nbsp;<a href="home.html">Home</a><br>
        &bull;&nbsp;&nbsp;<a href="home.html#about">About LTS</a><br>
        &bull;&nbsp;&nbsp;<a href="home.html#menu">Our Menu</a><br>
        &bull;&nbsp;&nbsp;<a href="hours.html">Store Hours</a><br>
    </section>
    
    <br>
    <a href="/img/tacos_close_up_400x260.png">
        <img src="/img/tacos_close_up_400x260.png" height="400">
    </a>
    <br>
    
    <h5>Little Tacos Shop Tacos</h5>

    <section id="contact-form">
    <h2>Our Contact Form</h2>
    <div class="contact-frame">
        <h5 style="position: absolute; top: 0px; left: 20px; margin: 0;">Send Us a Message</h5>
        <form>
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" placeholder="Type your name here..." required>

            <label for="email">Email:</label>
            <input type="email" id="email" name="email" placeholder="Type your email here..." required>
            
            <label for="message">Your Message:</label>
            <textarea id="message" name="message" placeholder="Type your message here..." required></textarea>

            <button type="submit" class="send-button">Send</button>
            <button type="reset" class="reset-button">Reset</button>
        </form>
    </div>
    </section>

    <section id="location">
        <h2>Our Location</h2>
        <p><em>555 Taco Temptation Lane, Suite T</em></p>
        <p><em>Kansas City, MO 55555-5555</em></p>
        <p><em>Phone: 555-555-5555</em></p>
        <p><em>Phone: <a href="tel:5555555555">555-555-5555</a></em></p>
    </section>
    
    <hr> 
    <a href="#contact">Back to Top</a>
    <p>&copy; The Little Taco Shop</p>
</body>
</html>
=============
Note. It looks like that I cant position the "<h5>Send Us a Message</h5>" in the frame border.
----
I will now play the lesson10 tutorial and see how Dave Gray was able to build the three web pages.
Chapter 10 HTML Full Course for Beginners | Complete All-in-One Tutorial | 4 Hours
https://youtu.be/mJgBOIoGihA?si=xveW0gRatTmQz1Jk&t=12303
-----
Added <html lange="en"> to contact.html. hours.html file okay.

add the following two lined to <head> of index.html
<link rel="icon" href="favicon.ico" type="image/x-icon">
<link rel="stylesheet" href="css/style.css">
----
Note somewhere along the line I changed index.html to home.html
So I recreated file index.html and copied home.html
I will need to fix page links in contact.html and hours.html tp fix navigation.
Page Navigation links have now been fixed.
-----
added:
    <meta name="author" content="original tutorial by Dave Gray, content rebuilt by Rascus using VSCodeand and chatGPT4">
    <meta name="description" content="The Little Taco Shop landing page">
-----
resume video here
https://youtu.be/mJgBOIoGihA?si=sS_S3Dt1feit9hva&t=13520
---contact form---
Explore this website: https://httpbin.org/#/HTTP_Methods

<main>
	<form action="https://httpbin.org/get" method="get:>
		<fieldset>
			<legend>Send Us A Messsage</legend>
		</fieldset>
	</form>
</main>
<hr>
<footer>
	<p>Copyright &Copy; The Little Taco Shop</p>
</footer>
------indx.html----
ask chatGPT4:
emphasis on "love of Tacos" 
<p>LTS was founded in 2022. Our shop was built from a love of tacos.</p>
---
Sure! Here’s a revised version that emphasizes the love of tacos:

<p>LTS was founded in 2022, born from an **unwavering passion for tacos**. Our shop is a celebration of this love, where every dish is crafted with dedication and joy.</p>
---
Here you go:

<p>LTS was founded in 2022. Our shop was built from a **love of Tacos**.</p>
---
make bold text "love of Tacos"  
<p>LTS was founded in 2022. Our shop was built from a love of Tacos.</p>
---
Okay, so ask chatGPT4 to:
help me create a html page to show "<p>LTS was founded in 2022. Our shop was built from a love of tacos.</p>" add css  style to format "love of Tacos" as bold text
----
Here’s a simple HTML page with CSS to emphasize "love of Tacos" in bold:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Love of Tacos</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f8f9fa;
            color: #333;
            padding: 20px;
            text-align: center;
        }
        .highlight {
            font-weight: bold;
            color: #d9534f; /* Optional: a taco-inspired color */
        }
    </style>
</head>
<body>
    <p>LTS was founded in 2022. Our shop was built from a <span class="highlight">love of Tacos</span>.</p>
</body>
</html>
```

Feel free to customize the styles as needed!
---index.html----
append to <Style>
.highlight {
    font-weight: bold;
    color: #d9534f; /* Optional: a taco-inspired color */
}
edit code to highlight selected text:
change 
<p>LTS was founded in 2022. Our shop was built from a love of Tacos.
to:
<p>LTS was founded in 2022. Our shop was built from a <span class="highlight">love of Tacos</span>.
-------
Side note re style.css file versus CSS style code in separate web pages.
I tried to move all the <Style> code from index.html into style.css, however, this affected the form frame/box outline around the form elements. Similarly, the same issue happened with the emphasis on "love of Tacos"
The advantage of consolidating <style> code into a single file is that it reduces the number of http requests on the backend server and allows web pages to load faster from client side cache memory if they already exist.
----contact.html----
send form contact information to http://httpbin.org test website.

Here's an updated version of your HTML page that sends form data to "https://httpbin.org/post" when the submit button is clicked:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="author" content="original tutorial Dave Gray, content rebuilt by Rascus using VSCode and chatGPT4">
    <meta name="description" content="The Little Taco Shop Contact form">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Us</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            padding-left: 20px;
            padding-right: 20px;
        }
        #hours {
            margin: 20px;
        }
        img {
            max-width: 100%;
            height: auto;
        }
        .contact-frame {
            width: 100%;
            height: 50vh;
            border: 1px solid #ccc;
            padding: 20px;
            box-sizing: border-box;
            position: relative;
        }
        h1, h2 {
            margin: 20px 0;
        }
        label {
            display: block;
            margin: 10px 0 5px;
        }
        input[type="text"],
        input[type="email"],
        textarea {
            width: 33%;
            margin: 10px 0;
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
            display: block;
        }
        textarea {
            height: 100px;
            resize: none;
        }
        button {
            margin: 10px 5px;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .send-button {
            background-color: #4CAF50;
            color: white;
        }
        .reset-button {
            background-color: #f44336;
            color: white;
        }
    </style>
</head>
<body>
    <section id="hours">
        <h1>Contact Us</h1>
        &bull;&nbsp;&nbsp;<a href="index.html">Home</a><br>
        &bull;&nbsp;&nbsp;<a href="index.html#about">About LTS</a><br>
        &bull;&nbsp;&nbsp;<a href="index.html#menu">Our Menu</a><br>
        &bull;&nbsp;&nbsp;<a href="hours.html">Store Hours</a><br>
    </section>
    
    <br>
    <a href="/img/tacos_close_up_400x260.png">
        <img src="/img/tacos_close_up_400x260.png" height="400">
    </a>
    <br>
    
    <h5>Little Tacos Shop Tacos</h5>

    <section id="contact-form">
    <h2>Our Contact Form</h2>
    <div class="contact-frame">
        <h5 style="position: absolute; top: 0px; left: 20px; margin: 0;">Send Us a Message</h5>
        <form action="https://httpbin.org/post" method="POST">
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" placeholder="Type your name here..." required>

            <label for="email">Email:</label>
            <input type="email" id="email" name="email" placeholder="Type your email here..." required>
            
            <label for="message">Your Message:</label>
            <textarea id="message" name="message" placeholder="Type your message here..." required></textarea>

            <button type="submit" class="send-button">Send</button>
            <button type="reset" class="reset-button">Reset</button>
        </form>
    </div>
    </section>

    <section id="location">
        <h2>Our Location</h2>
        <p><em>555 Taco Temptation Lane, Suite T</em></p>
        <p><em>Kansas City, MO 55555-5555</em></p>
        <p><em>Phone: 555-555-5555</em></p>
        <p><em>Phone: <a href="tel:5555555555">555-555-5555</a></em></p>
    </section>
    
    <hr> 
    <a href="#contact">Back to Top</a>
    <p>&copy; The Little Taco Shop</p>
</body>
</html>
```

### Key Changes:
- The `<form>` tag now includes `action="https://httpbin.org/post"` and `method="POST"` attributes to send data to the specified URL when the form is submitted.
-----test contact.html submit data ----
https://httpbin.org/post
{
    "args": {},
    "data": "",
    "files": {},
    "form": {
        "email": "spock@gremlon.com",
        "message": "Watchout the gremlims are gathering!!!",
        "name": "Spock Gremlin"
    },
    "headers": {
        "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
        "Accept-Encoding": "gzip, deflate, br, zstd",
        "Accept-Language": "en-US,en;q=0.9,en-AU;q=0.8",
        "Cache-Control": "max-age=0",
        "Content-Length": "97",
        "Content-Type": "application/x-www-form-urlencoded",
        "Host": "httpbin.org",
        "Origin": "http://127.0.0.1:5500",
        "Priority": "u=0, i",
        "Referer": "http://127.0.0.1:5500/",
        "Sec-Ch-Ua": "\"Chromium\";v=\"130\", \"Microsoft Edge\";v=\"130\", \"Not?A_Brand\";v=\"99\"",
        "Sec-Ch-Ua-Mobile": "?0",
        "Sec-Ch-Ua-Platform": "\"Windows\"",
        "Sec-Fetch-Dest": "document",
        "Sec-Fetch-Mode": "navigate",
        "Sec-Fetch-Site": "cross-site",
        "Sec-Fetch-User": "?1",
        "Upgrade-Insecure-Requests": "1",
        "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/130.0.0.0 Safari/537.36 Edg/130.0.0.0",
        "X-Amzn-Trace-Id": "Root=1-6716f2a1-01a3eb903ed5c2560ec16c8b"
    },
    "json": null,
    "origin": "43.252.108.236",
    "url": "https://httpbin.org/post"
}
-----
Revisit Taco Trivia
<aside>
	<h3>Taco Trivia</h3>
	<details>
		<summary>When did tacos first appear in the United States></summary>
		     <p>
                        Jeffrey M. Pilcher, taco historian and professor of history at the University of Minnesota, says
                        the earliest mention of tacos in the United States are in a newspaper from <time
                            datetime="1905">1905</time>. (Source: <cite><a
                                href="https://www.smithsonianmag.com/arts-culture/where-did-the-taco-come-from-81228162/"
                                target="_blank">Smithsonian Magazine</a></cite>)
                    </p>
	</details>
</aside>
========