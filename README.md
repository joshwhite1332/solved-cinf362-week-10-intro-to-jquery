Download Link: https://assignmentchef.com/product/solved-cinf362-week-10-intro-to-jquery
<br>
<strong>Agenda</strong>

<ul>

 <li>Introduction to JQuery

  <ul>

   <li>What is JQuery?</li>

   <li>Class Example</li>

   <li>JQuery Challenges</li>

   <li>JavaScript Features Discussion</li>

  </ul></li>

 <li>Next Week</li>

</ul>




<h2>Introduction to JQuery</h2>

<strong>What is it?</strong>

JQuery is a library based on JavaScript that allows users to implement the same features they would in JavaScript but with less code. Things like DOM manipulation, event handling, animation, and more can be done more easily. It comes in multiple flavors such as JQuery core, JQuery UI (for widgets like accordions, tabbed layouts, etc.), and JQuery Mobile (for use with creating responsive websites). The one we will focus on for this course is JQuery core, but you can use any of them if you’d like except for JQuery Mobile (your responsive design should be done with media queries).




You can use JQuery on your page by either downloading a copy of the JQuery code and linking it like regular external JS or by using JQuery hosted on a Content Delivery Network (CDN). For the purposes of this course, you can do either. The main advantage to using JQuery hosted by Google or some other platform is that a user won’t have to download the code again if it was already downloaded from another website they visited.




One downside to JQuery is that it adds a bit of bloat to your code. Usually, to use any one feature, you still must download the whole library which can add a lot of unnecessary code to your page. In most instances, you can build the feature with plain JS but if it’s more complex, JQuery can be helpful. Despite the code bloat, JQuery is still a very small library and with modern bandwidth limits, it might not be an issue to have a local copy.




The CDN I recommend/will be using in my class examples comes from Google and is displayed below. You would add this directly before your own script tag in order to use it as depicted.




&lt;script src=”https://ajax.googleapis.com/ajax/libs/jquery/3.4.1/jquery.min.js”&gt;&lt;/script&gt;

&lt;script src=”script.js”&gt;&lt;/script&gt;




One major difference in JQuery is how you can select items on the page. Rather than use the standard document.getElementById or document.querySelector methods, we can simply use a dollar sign and specify the html element, class, id, attribute, etc.




With regular JS, we might use the following code to add a click event to a button:




&lt;button id=“btn”&gt;Submit&lt;/button&gt;

document.getElementById(“btn”).onclick = function() {// function code }




In JQuery, we can simply say:




$(“#btn”).click(function() {//function code});




The dollar sign is built in as a selector for all types of stuff. The only thing you need to do is specify by element, class name, id name, etc. The selectors work the same as they do in CSS so if you want to select a class, you must identify it with a period. The same goes for ids with the pound sign (#). There are two basic examples below but JQuery is very robust with the criteria it can use to select elements.




Selecting a class of para inside a div: $(“div.para”)

Selecting a list item inside of an unordered list: $(“ul li”)




There’s so much more to JQuery but rather than explain the technical details here, I’ve provided links to various resources that will demonstrate some of its capabilities. You don’t have to read through all of them, feel free to skim through them to see what features are available. Additionally, the class example contains my own code in addition to more explanations that will be relevant for this week’s assignment.




<u>Additional Resources</u>

<ul>

 <li><a href="https://jquery.com/">https://jquery.com/</a> (General JQuery Website)</li>

 <li><a href="https://api.jquery.com/">https://api.jquery.com/</a> (Technical details for JQuery core)</li>

 <li><a href="https://learn.jquery.com/">https://learn.jquery.com/</a> (Learn about JQuery core)</li>

 <li><a href="https://www.tutorialspoint.com/jquery/jquery-overview.htm">https://www.tutorialspoint.com/jquery/jquery-overview.htm</a> (Multiple sections)</li>

</ul>

<strong><u>Class Examples:</u></strong>

<a href="https://iinf362.000webhostapp.com/examples/">https://iinf362.000webhostapp.com/examples/</a> (All examples for the course)

<a href="http://iinf362.000webhostapp.com/examples/jquery/">http://iinf362.000webhostapp.com/examples/jquery/</a> (This week’s example)

Right-click this page in order to view the page source. I’ve left comments throughout the JavaScript to help you understand what is going on. These examples will help you with the challenges for this week’s assignment.




<strong><u>If you haven’t done so already, please read the “Creating and Viewing our Web Pages.docx” file on Blackboard. You will not be able to submit anything for the assignment without completing that portion first. </u></strong>




<strong>JQuery Challenges</strong>

Download the “JQuery-Challenges.zip” folder from Blackboard under the Lecture Notes for this week or in the Assignments folder. Inside of this zip folder, you’ll find an HTML file, a js folder, and a script.js file. Using these files, your task is to add JS to complete the challenges as they are described in the HTML file. In total, there are 5 main challenges that are short. Feel free to reference the class example code as it has items that will directly help you with this assignment.

<u> </u>

To receive credit for these challenges, submit a link to your JQuery Challenges page by <u>Wednesday, April 8<sup>th</sup> at midnight</u>. The assignment with be called JQuery Challenges in the assignments folder. It will also be accessible through the Lecture Notes for this week.




<strong>JavaScript Features Discussion</strong>

<u>Initial Post Due April 5<sup>th</sup> at Midnight</u>

Visit a few websites and go through their content on different devices and browsers (Google Web Tools can emulate some devices). While surfing the pages, pay attention to the various features and interactive components present on each page. Based on a little research and your current knowledge of JS/JQuery, describe in pseudo-code how you would recreate 3 unique components you find. You can research the components and look up how to code them. However, there is no actual coding required for your initial or response posts. I’ve given you some potential points for discussion to get you started in addition to examples of the type of posts I’d like to see. The discussion area on Blackboard will be titled JavaScript Features Discussion.




<ul>

 <li>What is the component or feature?</li>

 <li>What HTML elements are needed?</li>

 <li>What kind of event handler is being used?</li>

 <li>What types of data are being used?

  <ul>

   <li>string, array, numbers, etc.</li>

  </ul></li>

 <li>What would your function structure be?

  <ul>

   <li>Loops, if/else statements, arrays, etc.</li>

  </ul></li>

 <li>What parts are you not sure how to do?</li>

</ul>




<u>Response Post Due April 8<sup>th</sup> at Midnight</u>

Visit a website another student has mentioned, find another unique component not already discussed, and briefly describe it with pseudo-code using the guidelines above. Also, look at the pseudo-code provided by the student; do you agree with how they structured it? Are there other ways to achieve the same results? In your discussion, try to be as specific as possible with mentioning JS concepts.




<strong>Example Discussion Posts</strong>

<u>Initial Post: </u>

I visited madtakes.com and found an interactive game similar to mad libs. The user is supposed to type in words based on criteria such as nouns, verbs, or adjectives. When they submit their words, a story is generated using those words. To build this, you would need several inputs, labels, and buttons. I would use an onclick event handler to detect the user submission. After everything is submitted, I could then grab the values for each input and check them with .value() and an if else statement. If they weren’t empty, I would store each word as its own variable. The various stories could be saved as strings with the inputs being placed in them with concatenation like this “There once was a ” + word1 + “ in a giant castle.” To output the results, I would use .innerHTML with the previously created string.




<u>Response:</u>

I found another interesting component on your page in the navigation menu. Whenever the screen gets small enough, the links in the header collapse into a hamburger menu. To make that, I think you would need some sort of function to check for the window’s width. We could use an if/else statement to check the width and if it was below a certain width, we’d then use the .css() method in JQuery to alter the heading. Maybe we use JS to hide the original nav menu and display the new one.

Another way to do your mad libs code might be with arrays. Instead of storing each input as its own variable, maybe you use an array to store all of them. You could then resort the array and change the order of the words for every story. I’m not exactly sure how you would test for nouns vs verbs but maybe a dictionary could be imported.