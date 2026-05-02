4. createElement + append + remove (you used partly 👍)

You’ve done this a bit, but make it stronger:

let li = document.createElement("li");
li.textContent = "New Item";

document.getElementById("list").appendChild(li);

Remove:

li.remove();
_____________________________________________________________________________________
Form Handling (VERY important)
<form id="form">
    <input type="text" id="name">
    <button type="submit">Submit</button>
</form>
document.getElementById("form").addEventListener("submit", function(e) {
    e.preventDefault(); // stops page reload
    let value = document.getElementById("name").value;
    console.log(value);
});

👉 This is used everywhere (login forms, search bars)
__________________________________________________________________________________________
setTimeout & setInterval
setTimeout(() => {
    alert("Hello after 2 seconds");
}, 2000);
setInterval(() => {
    console.log("Running...");
}, 1000);

👉 Useful for:

timers
animations
auto updates
___________________________________________________________________________________________
1.

Create a paragraph with text "Click to change me".
Add a button, and when clicked:

change the text to "Text updated successfully"
change the color to blue
2.

Create an input box and a button.
When the button is clicked:

display the entered text in an h3 tag
if the input is empty, show "Please enter something"
3.

Create a list (ul) with 3 default items.
Add a button:

when clicked, it should duplicate all list items (same items added again)
4.

Create a button "Toggle Message"

when clicked once → show a message
when clicked again → hide the message

(Hint: use style.display)

5.

Create:

an input box
an "Add" button
a "Clear All" button

Functions:

Add button → adds items to list
Clear All → removes all items from the list
___________________________________________________________________________________
1. Change paragraph text and color
<!DOCTYPE html><html><head>    <title>Q1</title></head><body><p id="para">Click to change me</p><button onclick="changeText()">Change</button><script>function changeText() {    let p = document.getElementById("para");    p.innerText = "Text updated successfully";    p.style.color = "blue";}</script></body></html>

✅ 2. Input → display in h3 (with validation)
<!DOCTYPE html><html><head>    <title>Q2</title></head><body><input type="text" id="inputBox" placeholder="Enter text"><button onclick="showText()">Submit</button><h3 id="output"></h3><script>function showText() {    let value = document.getElementById("inputBox").value;    if (value === "") {        document.getElementById("output").innerText = "Please enter something";    } else {        document.getElementById("output").innerText = value;    }}</script></body></html>

✅ 3. Duplicate list items
<!DOCTYPE html><html><head>    <title>Q3</title></head><body><ul id="list">    <li>Item 1</li>    <li>Item 2</li>    <li>Item 3</li></ul><button onclick="duplicateItems()">Duplicate</button><script>function duplicateItems() {    let list = document.getElementById("list");    let items = list.innerHTML;    list.innerHTML += items;}</script></body></html>

✅ 4. Toggle message (show/hide)
<!DOCTYPE html><html><head>    <title>Q4</title></head><body><button onclick="toggleMessage()">Toggle Message</button><p id="msg" style="display:none;">Hello! This is a message</p><script>function toggleMessage() {    let msg = document.getElementById("msg");    if (msg.style.display === "none") {        msg.style.display = "block";    } else {        msg.style.display = "none";    }}</script></body></html>

✅ 5. Add items + Clear all
<!DOCTYPE html><html><head>    <title>Q5</title></head><body><input type="text" id="inputBox" placeholder="Enter item"><button onclick="addItem()">Add</button><button onclick="clearAll()">Clear All</button><ul id="list"></ul><script>function addItem() {    let value = document.getElementById("inputBox").value;    if (value !== "") {        let li = document.createElement("li");        li.innerText = value;        document.getElementById("list").appendChild(li);    }}function clearAll() {    document.getElementById("list").innerHTML = "";}</script></body></html>