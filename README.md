# JS211BlogPosts
<h2>Class 4: Prompt 202 - September 7</h2>
<b>1. What's something that's been confusing? How would you explain it to someone else?</b>
<p></p>
<b>2. What is "use strict";? What are the advantages and disadvantages to using it?</b>
<p><code>"use strict";</code> is a direction in JavaScript that enables "strict mode" in a script or function. It helps developers write error-free JavaScript code by catching common coding mistakes and preventing the use of problematic features.<code>"use strict";</code> is used for updating existing code to improve quality and catch potential bugs. Strict mode might not be supported in older browsers or environments and can also make it more difficult to write code if you're not used to writing code to adher to stricter rules.</p>
<b>3. Explain function hoisting in JavaScript.</b>
<p></p>
<b>4. Explain the importance of standards and standards bodies like ECMA.</b>
<p></p>
<b>5. What actions have you personally taken on recent projects to increase maintainability of your code?</b>
<p></p>
<b>6. Why is it, in general, a good idea to leave the global scope of a website as-is and never touch it?</b>
<p></p>
<h2>Class 2: Prompt 201 - August 31</h2>
<b>1. Describe one thing you're learning in class today.</b>
<p>I learned how the <code>!</code> (not) operator worked, which took some time but ultimately I got there. Also, I learned that JavaScript will actually accept a string even if there's an expected number value. In today's example, it was checking whether <code>num1 > 0</code> was <code>true</code> or <code>false</code>  Me and the rest of my classmates thought that if <code>num1 = "7"</code> (a string) and not <code>num1 = 7</code> (a number) that the function would mark it as false. However, it accepted it even though it was a string value.</p>
<b>2. What is the difference between <code>==</code> and <code>===</code> ?</b>
<p> <code>==</code> will accept two different data types, like a string and a number, as long as they contain the same value, like <code>"7"</code> and <code>7</code>. <code>===</code> is more precise, in that it will only accept two matching values and data types. </p>
<b>3. What is the value of <code>foo</code> in <code>var foo = 10 + '20'?</code></b>
<p>The value is <code>1020</code>, because <code>10</code> is a number and <code>'20'</code> is a string but you're using the <code>+</code> operator, JavaScript concatenates the two different data types. However, were this a function testing whether <code>'20'</code>  was greater than <code>10</code>, despite knowing <code>'20'</code> is a string, JavaScript would still evaluate it like a number and mark the function as "true". </p>
<b>4. Describe what a terminal application is.</b>
<p>A terminal application is a desktop app or extension (if you're using VS code) that lets you access the Shell. The Shell is a non GUI environment where you can write or access command lines, and you can think of it as the super techy looking interface you see in any movie or TV show about coders or hackers. The command line is the actual "code" that you write in the shell. Anything from <code>git add . </code>(add all files to the queue) to <code>cd</code> (change directory, meaning change folders) to <code>node main.js</code> (run the node.js program "main"). Examples of various terminal applications are Bash, PowerShell, or if you're on a Mac, just "Terminal". </p>
<b>5. What is the ternary operator?</b>
<p>Ternary operators are conditionals expressed as <code>?</code> and <code>:</code> that can be a more concise replacement for <code>if</code> <code>else</code>conditions (because they can be read easily as one line instead of 2). The <code>?</code> is followed by the value if the condition is  <code>true</code> , and the <code>:</code> is followed by the condition if  <code>false</code>.  One huge advantage is that while <code>const</code> variables can't be changed after declared, you could use a ternary operator within a <code>const</code> variable to apply different values to that variable depending on conditions. You can also use the ternary operators more traditionally as part of a function. 
<br>
Example as a <code>const</code> variable: <code>const legalAgeCategory = (age >= 18) ? "Adult" : "Minor";</code>
<br>
Example as a function: <code>const legalAgeCategory = (age) => {return age >=18 ? "Adult" : "Minor"}</code>
</p>
<b>6. What are some ways to ensure that your website design or web application is accessible and user-friendly?</b>
<p>Adding alt text to <code>img</code> elements can help ensure it's accessible. Also heavily limiting or completely excluding iFrames is very helpful and more user-friendly.</p>
<b>7. What are your favorite features of HTML5, and how have you implemented them in your front-end development projects?</b>
<p>Simple things such as semantic elements like <code>nav</code> have been instrumental for making even basic websites (you need a navigation bar!) and I've taken much advantage of the improved form structures like <code>required</code> as an attribute and the automatically formatted <code> &#60;input type=""&#62;</code> has been extremely helpful for email and date fields. </p>
<b>8. How do you structure your CSS and JavaScript to make it easier for other developers to work with?</b>
<p>Writing comments is exceedingly important, but also naming your variables in JavaScript in descriptive and accurate ways can help others understand. Also avoiding using ternary operators unless the purpose of the function or variable is very obvious, as it can make it harder to read and understand what's going on. </p>
<b>9. What's your process for addressing browser-specific rendering problems? Do you find that a certain browser is more challenging to work with than others?</b>
<p>The first step is to test the website or application on different browsers (Edge, Chrome, Safari, etc.) and then adjust as needed. Using standard HTML5 structure and W3 best practices can help ensure that for the most part there aren't huge rendering issues. I haven't worked with enough browsers to have a strong opinion, but the work <a href="https://www.vox.com/2018/5/3/17309078/digital-art-diana-a-smith-francine-coded-browser-art">CSS Francine</a> would imply that an old version of Opera or Internet Explorer 7 would drastically change the way CSS is rendered.</p>
