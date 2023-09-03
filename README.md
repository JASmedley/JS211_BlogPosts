# JS211BlogPosts
<h2>Class 2: Prompt 201 - August 31</h2>
<b>1. Describe one thing you're learning in class today.</b>
<p>I learned how the ! (not) operator worked, which took some time but ultimately I got there. Also, I learned that JavaScript will actually accept a string even if there's an expected number value. In today's example, it was checking whether num1 > 0 was true or false. Me and the rest of my classmates thought that if num1 = "7" (a string) and not num1 = 7 (a number) that the function would mark it as false. However, it accepted it even though it was a string value.</p>
<b>2. What is the difference between == and === ?</b>
<p> == will accept two different data types, like a string and a number, as long as they contain the same value, like "7" and 7. === is more precise, in that it will only accept two matching values and data types. </p>
<b>3. What is the value of foo in var foo = 10 + '20'?</b>
<p>The value is 1020, because 10 is a number and 20 is a string but you're using the + operator, JavaScript concatenates the two different data types. However, were this a function testing whether '20' was greater than 10, despite knowing '20' is a string, JavaScript would still evaluate it like a number and mark the function as "true". </p>
<b>4. Describe what a terminal application is.</b>
<p></p>
<b>5. What is the ternary operator?</b>
<p>Ternary operators are conditionals expressed as ? and : that can be a more concise replacement for if/else conditions (because they can be read easily as one line instead of 2). The ? is followed by the value if the condition is true, and the : is followed by the condition if false. One huge advantage is that while const variables can't be changed after declared, you could use a ternary operator within a const variable to apply different values to that variable depending on conditions. You can also use the ternary operators more traditionally as part of a function. 
Example as a const variable: const legalAgeCategory = (age >= 18) ? "Adult" : "Minor";
Example as a function: const legalAgeCategory = (age) => {return age >=18 ? "Adult" : "Minor"}
</p>
<b>6. What are some ways to ensure that your website design or web application is accessible and user-friendly?</b>
<p>Adding alt text to img elements can help ensure it's accessible. Also heavily limiting or completely excluding iFrames is very helpful and more user-friendly.</p>
<b>7. What are your favorite features of HTML5, and how have you implemented them in your front-end development projects?</b>
<p></p>
<b>8. How do you structure your CSS and JavaScript to make it easier for other developers to work with?</b>
<p>Writing comments is exceedingly important, but also naming your variables in JavaScript in descriptive and accurate ways can help others understand. Also avoiding using ternary operators unless the purpose of the function or variable is very obvious, as it can make it harder to read and understand what's going on. </p>
<b>9. What's your process for addressing browser-specific rendering problems? Do you find that a certain browser is more challenging to work with than others?</b>
<p></p>
