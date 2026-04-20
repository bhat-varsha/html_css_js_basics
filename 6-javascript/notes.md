JavaScript is a programming language for the browser

It is used to:

Make pages interactive
Handle button clicks
Change text, images, forms
Talk to backend (later)
_________________________________________________________________
JavaScript = makes your page do things

Without JS:Button = just looks clickable ❌

With JS:Button can change text, show message, update page ✅
_________________________________________________________________
JavaScript = makes page interactive
Variables = store data
Data types = kind of data
Functions = reusable logic
Operators = calculations
DOM = control HTML
Events = user actions
_________________________________________________________________

Technology	        Role
HTML	            Structure (skeleton)
CSS / Tailwind	    Design (looks)
JavaScript	        Behavior (actions)
_________________________________________________________________
by usinf form we have cretaed the input and the button which will submit , but without js the button will not work
for dynamic(changing)nature of webpages or browser we use javascript

Without JS:
👉 Button does nothing

With JS:
👉 Button can:

Show alert
Change text
Add data
_________________________________________________________________
Variables = containers to store values
 Syntax : let name = "varsha";

Types of variables
1. let (most used)  Value can change
let age = 20;

2. const   Value cannot change
const pi = 3.14;
_________________________________________________________________
Functions 
Function = block of code that runs when called

the fucntguon name can be anything
function sayHello() {}
function abc() {}
function varshaFunction() {}

button onclick="sayhello()"
the onclick is builtin we have to use the same , but the sayhello which is fucntion (action which will do )
can be anything
fucntion name does not display in webpages
_________________________________________________________________
inbuilt event
Event	When it happens
onclick	When user clicks
onchange	When input value changes
oninput	When typing in input
onmouseover	When mouse comes over element
onmouseout	When mouse leaves
onkeydown	When key is pressed
onload	When page loads

<input oninput="sayHello()">
👉 When user types → function runs
_________________________________________________________________
documnet.getElementbyId=“Go to HTML and get this element”
addEventListener() Purpose: ADD action to element

getElementById → find the button or getElementById to find the element you want to CHANGE
ONLY when you want to CHANGE or ACCESS an element

Reason 1: To CHANGE something
document.getElementById("title").innerText = "new"
✅ Reason 2: To ATTACH event (addEventListener)
let btn = document.getElementById("btn");

addEventListener → tell button what to do

_________________________________________________________________
JavaScript	What it does

document.getElementById('name4').style.color = "red";


.style.color = "red"	Text color
.style.backgroundColor = "yellow"	Background
.style.fontSize = "20px"	Font size
.style.display = "none"	Hide element
.style.display = "block"	Show element
.style.border = "1px solid black"	Border
.style.padding = "10px"

_________________________________________________________________
DOM properties/methods

Most Important DOM Things (Must Know)
🔹 1. innerText : Changes only text
element.innerText = "Hello";

🔹 2. innerHTML : Can include HTML
element.innerHTML = "<b>Hello</b>";

🔹 3. value (VERY IMPORTANT for forms) Gets input value
document.getElementById("input1").value

🔹 4. style  : Changes design
element.style.color = "red";

🔹 5. setAttribute() : Adds/changes attribute
element.setAttribute("class", "bg-red-500");

🔹 6. getAttribute() : Gets attribute value
element.getAttribute("id");


🔹 7. appendChild()  : Adds new element
parent.appendChild(child);

🔹 8. remove() : Deletes element
element.remove();
