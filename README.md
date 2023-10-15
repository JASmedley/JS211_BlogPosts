# JS211BlogPosts
<h2>Class 14: Prompt 207 - October 12</h2>
<b>1. Write about something you learned this week.</b>
<p></p>
<b>2. Why would you use something like the load event? Does this event have disadvantages? Do you know any alternatives, and why would you use those?</b>
<p></p>
<b>3. What are the advantages and disadvantages of using Ajax?</b>
<p></p>
<b>4. Explain how JSONP works (and how it's not really Ajax).</b>
<p></p>
<b>5. Explain Ajax in as much detail as possible.</b>
<p></p>
<b>6. What does it mean when we talk about time complexity of an algorithm?</b>
<p></p>
<b>7. What are the three laws of algorithm recursion?</b>
<p></p>
<b>8. How do you see yourself growing as a web developer?</b>
<p></p>

<h2>Class 12: Prompt 206 - October 5</h2>
<b>1. Tell us about something you learned this week.</b>
<p>I learned about bubble sorting vs binary sorting, which was very informative because I kind of understood bubble sort but did not understand why it was slow and ineffective. Then seeing the animation of how it works it becamse clear that using bubble sort is like watching paint dry. Then we did binary sorting, which is the opposite of bubble sorting in that conceptually it sounds a lot slower, but in practice is much faster (for a computer at least, for a human this would be so much longer than randomly flipping through something). </p>
<b>2. What are the pros and cons of immutability?</b>
<p>
  <h3>Pros</h3>
  <ul>
    <li><b>Predictable:</b> They're predictable because they don't change after they're created so you always know how they're going to work</li>
    <li><b>Debuggable:</b> Because of the point above, this makes them easier to debug</li>
  </ul>
  <h3>Cons</h3>
  <p>
    <ul>
    <li><b>Learning Curve:</b> For developers transitioning from mutable to immutable programming paradigms, there might be a learning curve. </li>
    <li><b>Memory Usage:</b> If you use too many immutable objects, you have to keep creating a bunch more to accomplish what you want, that uses up more memory.</li>
  </ul>
 </p>
<b>3. How can you achieve immutability in your own code?</b>
<p> You can use a <code>const</code> variable when you want to create an immutable variable. However, as a whole, JavaScript doesn't have immutable maps and lists so you would need to use a third-party script like immutable.js. However, immutable.js was written by developers at Facebook, the company that crashed for an entire day because someone got their border gateway protocol wrong, so maybe don't trust it too much.</p>
<b>4. What are Divide and Conquer algorithms? Describe how they work. Can you give any common examples of the types of problems where this approach might be used?</b>
<p>Divide and conquer algorithms break larger problems into smaller subproblems. They keep breaking down the related subproblems until they become simple enough to be solved directly. Merge Sort is an example of a Divide and Conquer algorithm. 
  <ul>
  <li><b>Divide:</b> Split the unsorted list into sublists of related elements</li>
  <li><b>Conquer:</b> Sort the sublists.</li>
  <li><b>Combine:</b> Merge the sorted sublists to produce a new sorted list.</li>
  </ul>
</p>
<b>5. How do insertion sort, heap sort, quick sort, and merge sort work?</b>
<p>
  <ul>
    <li><b>Insertion Sort:</b> Builds an already sorted array one element at a time.</li>
    <li><b>Heap Sort:</b> Builds a binary tree where the parent nodes are greater than or equal to their children then takes the larges element and puts it at the end of the array. </li>
    <li><b>Quick Sort:</b> Takes an element and puts it into two sublists (sub arrays), 1. elements less than the original and 2. elements greater than the original. It then sorts the sublists.</li>
    <li><b>Merge Sort:</b> Takes an unsorted array and creates subarrays with a single element then keeps merging the subarray elements until only one sorted array is left.</li>
  </ul>
</p>
<b>6. What are the key advantages of insertion sort, quick sort, heap sort and merge sort? Discuss best, average, and worst case time and memory complexity.</b>
<p>Insertion Sort is fastest for small datasets and already mostly sorted data. Quick Sort is the fastest general-purpose sorting algorithm in practice. Heap Sort is good for large datasets. Merge Sort is consistent but average, making it suitable for any other scenarios.</p>
<b>7. Explain the difference between mutable and immutable objects.</b>
<p>Mutable means that the objects can change, or be affected later in the code. Immutable objects are the opposite.</p>
<b>8. What are the three laws of algorithm recursion? Describe them in your own words and what they mean to you.</b>
<p>
  <ol>
    <li><b>Base Case Law:</b>Each recursive algorithm must have a base case, the emergency exit of a recursive function. It's a condition where the function stops making recursive calls and does something specifi.</li>
    <li><b>Law of Progress:</b>Each recursive call must be one step closer to reaching the base case. If each recursive call doesn’t get closer to a solution, the function might never reach the base case, violating the first law.</li>
    <li><b>Law of Design:</b>Each recursive algorithm must be able to solve a smaller subproblem of the original.</li>
  </ol>
</p>

<h2>Class 10: Prompt 205 - September 28</h2>
<b>1. Describe one thing you're learning in class today. Why do you think it will be important in your future web development journey?</b>
<p>I leanred how to build my own unit tests. Building tests is important, because if you're working for a company with proprietary information, you don't want to just plug it in to codepen.io for the world to see just to be able to test your work.</p>
<b>2. Can you offer a use case for the new arrow <code>=> </code>function syntax?</b>
<p>When storing a function in a <code>const</code> variable, so <code> const exampleFunction = (parameter) => {} </code></p>
<b>3. How does this new syntax differ from the older function signature, <code>function nameFunc(){}</code>, both in style and functionality?</b>
<p>The arrow code is written as <br>
<code>const nameFunc = () => { // function body };</code> <br>
while the older function is written as <br>
  <code>function nameFunc() {// function body} </code> <br>
The arrow syntax is more advantageous because it's more concise (can be written all on one line), <br>
<code>// Arrow function
const add = (a, b) => a + b;

// Traditional function
function add(a, b) {
  return a + b;
}
</code> and also it inherit's the `this` binding, unlike the older syntax where you have to define the function along with `this` for the binding to work. 
</p>
<b>4. Explain the differences on the usage of foo between <code>function foo() {}</code> and <code>const foo = function() {}</code></b>
<p> The first one is creating a function called <code>foo</code> and the second is creating a variable called <code>foo</code> that will contain a function.</p>
<b>5. What advantage is there for using the arrow syntax for a method in a constructor?</b>
<p>With arrow functions, you can define methods inside the constructor itself, and you can still use the `this` binding with them. </p>
<b>6.Can you give an example for destructuring an object or an array?</b>
<p><code>const person = {
  name: "Alice",
  age: 30,
  city: "New York"
};

// Destructuring the object
const { name, age, city } = person;</code></p>
<b>7.Explain Closure in your own words. How do you think you can use it? Don't forget to read more blogs and videos about this subject.</b>
<p>To first understand Closure it's important to understand "lexical scope". Lexical scope basically means the scope of a variable is determined by its position within the source code. Like a variable defined within a function will not operate the same way as a variable defined outside of a function. A closure is a mix of a function and the lexical scope within which that function was declared. It's basically when you declare the function one last time.</p>

<h2>Class 8: Prompt 204 - September 21</h2>
<b>1. Describe one thing you're learning in class today.</b><p></p>
<p>I learned that MasterMind is basically Wordle without words.</p>
<b>2. Can you describe the main difference between a forEach loop and a .map() loop and why you would pick one versus the other?</b>
<p>If you need to create a new array based on the original one, use .map(). If need to go through the array and perform some action without generating a new one, use forEach. So it depends on whether you need to transform data or just perform operations on it.</p>
<b>3. Describe event bubbling.</b>
<p>Event bubbling is a concept in JavaScript and DOMG that describes the order in which events are populated or "bubbled" up through the DOM hierarchy when an event occurs on a specific element. </p>
<b>4. What is the definition of a higher-order function?</b>
<p>Functions that take another function as one of their parameters.</p>
<b>5. ES6 Template Literals offer a lot of flexibility in generating strings. Can you give an example?</b>
<p>Yes, if you're trying to create a marketing email template and you have different variable information you want to include like the name of the person, their job title, etc. Instead of having to create one long <code>console.log</code> prompt with a series of commas and variables, you can write out the email and then just change the variales by adding <code>${}</code> around them.</p>
<b>6. What is an associative array in JavaScript?</b>
<p>Objects that have keys that reference each of the various values stored in the object. The keys and values together are called key-value pairs.</p>
<b>7. Why should you never use new Array in JavaScript?</b>
<p>When you create an array with new Array() and specify a length, you get a sparse array. A sparse array is one in which some indices have no assigned value.</p>
<h2>Class 6: Prompt 203 - September 14</h2>
<b>1. Describe one thing you're learning in class today.</b>
<p>I have a really strong understanding of for loops now. Before I was memorizing the structure but not really understanding how they worked, but doing a prime number example helped me better understand how to think through problems and also exactly how for loops work.</p>
<b>2. What's the difference between: <code>function Person(){}</code>, <code>var person = Person(),</code>, and <code>var person = new Person()</code>?</b>
<p>The first one is a function named "Person", the second one is a variable called "person" storing the function Person in it. The third one is altering the valueable person by adding a new blank property to the function Person.</p>
<b>3. What's the difference between an "attribute" and a "property"?</b>
<p>Attributes are the information pieces specific to the properties in an element in the DOM, and the properties are the applicable generic qualities. Basically, if you have an element that's <code>input type ="text"</code> then the property is <code>type</code> and the attribute is <code>"text"</code></p>
<b>4. What language constructions do you use for iterating over object properties and array items?</b>
<p>
  For Arrays: 
<code>.slice()
.splice()
.toString()
.concat()
.includes()
.pop()
.push()
.join()
.length
.indexOf()
.shift()
.unshift()
.every()
.flat()
.find()
.reverse()
.forEach()
.map() 
</code>
</p>
<b>5. What is the event loop?</b>
<p>An event loop is something that pulls stuff out of the queue and places it onto the function execution stack whenever the function stack becomes empty.</p>
<b>6. What is the difference between call stack and task queue?</b>
<p> CallStack is a data structure which keeps track of function calls. Whenever we call a function, we are pushing it to the stack. Task queue is a different type of callback, it is dedicated to handling web API callbacks.</p>
<b>7. What are the differences between ES6 classes and ES5 function constructors?</b>
<p>ES6 class constructors creates objects by adding function to their prototypes. ES5 functions create objects and also an inheritance property.</p>

<h2>Class 4: Prompt 202 - September 7</h2>
<b>1. What's something that's been confusing? How would you explain it to someone else?</b>
<p>For loops have been confusing, specifically writing them. I've understood the logic better now, but I don't think there is much to explain for writing them other than to just write it once, and get used to writing or copying and pasting it and then switching out variables based on what you are trying to accomplish. </p>
<b>2. What is "use strict";? What are the advantages and disadvantages to using it?</b>
<p><code>"use strict";</code> is a direction in JavaScript that enables "strict mode" in a script or function. It helps developers write error-free JavaScript code by catching common coding mistakes and preventing the use of problematic features.<code>"use strict";</code> is used for updating existing code to improve quality and catch potential bugs. Strict mode might not be supported in older browsers or environments and can also make it more difficult to write code if you're not used to writing code to adher to stricter rules.</p>
<b>3. Explain function hoisting in JavaScript.</b>
<p>Function hoisting is when a function is referenced before it's actually defined. This works because the function definition is "hoisted" to the top of the current code, so it works as though it was defined before being referenced.
Example: </p>
<code>sayHello(); //function is referenced here, but hasn't been defined yet

  function sayHello() {
  console.log("Hello, world!");} //now the function has been defined
</code>
<br>
<b>4. Explain the importance of standards and standards bodies like ECMA.</b>
<p>The ECMA (European Computer Manufacturers Association) is one of the organizations responsible for creating and maintaining standards in JavaScript and other programming languages. They are the ones deciding on what will become deprecated, what new built-in functions should be added, and also they try to mitigate backwards compatibility. </p>
<b>5. What actions have you personally taken on recent projects to increase maintainability of your code?</b>
<p>One big thing for me is making sure my code is readable, I minimize accurately labeled functions that have been defined so that there is less code to look at when I go back to a project. This helps with the readability of it, and then I can also expand the functions to get a better understanding of how they operate. Giving the functions longer titles that describe what they do also makes it easier to understand the calls between functions. I try and comments that make sense to me, but I also delete out older comments that don't make senseo r that tend to crowd up the code. For me having less code to look at (even if it's commented out) makes it easier to understand and maintain the code. I also try and be consistent when writing functions, using the <code>const function = () => {} </code> method instead of the direct reference like <code>function thisFunction () {} </code> method. The consistency makese it easier to maintain.</p>
<b>6. Why is it, in general, a good idea to leave the global scope of a website as-is and never touch it?</b>
<p>The global scope is shared by all scripts, documents, and libraries on a website. When you start using global variables or functions, you increase the risk of naming conflicts or unintended interactions between different parts of your code. Like defining a function in the global scope that ends up interfering with a different function you write for a single web page later. By not using the global scope, you reduce the chances of these conflicts.</p>
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
