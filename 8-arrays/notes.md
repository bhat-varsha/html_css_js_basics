#               READ FROM 45 TH LINE FOR ARRAYS

1. Arrays : An array is used to store multiple values in one variable []
🔸 Syntax
let fruits = ["apple", "banana", "mango"];
console.log(fruits[0]); // apple
            Index starts from 0

🔹 2. Objects : An object stores data in key-value pairs {}
🔸 Syntax
let person = {
    name: "Varsha",
    age: 21,
    city: "Bangalore"
};
🔸 Access values
console.log(person.name);
console.log(person["age"]);

🔹 3. Loops : Loops are used to repeat code multiple times
🔸 for loop
for (let i = 0; i < 5; i++) {
    console.log(i);
}

🔹 4. Conditions : Conditions are used to make decisions in code
🔸 if statement
let age = 18;
if (age >= 18) {
    console.log("Adult");
}
🔸 if-else
if (age >= 18) {
    console.log("Adult");
} else {
    console.log("Minor");
}

Concept	Purpose
Array	store multiple values
Object	store structured data
Loop	repeat code
Condition	decision making
_____________________________________________________________________________________
An array in JavaScript is just a container that stores multiple values in one variable.

<script>
    let a = ["A","B","C"];
    console.log(a);
</script>

Example:
let a = ["A", "B", "C"];

Arrays are ordered
Index starts from 0
You can store strings, numbers, objects, etc.

Common operations:
a.push("D");   // add at end
a.pop();       // remove last
a[0];          // access first element
a.length;      // total elements

undertsand the code first ;
Q2: Delete Last Element
Add button to remove last element from array
function removeLast(){
    arr.pop();
}

✅ Q3: Search Element
Search if a value exists in array

function search(){
    let val = document.getElementById("gene").value;

    if(arr.includes(val)){
        alert("Found");
    } else {
        alert("Not Found");
    }
}
✅ Q4: Count Elements
function count(){
    alert("Total elements: " + arr.length);
}
✅ Q5: Display in Paragraph instead of List
function show(){
    let text = "";
    for(let i=0;i<arr.length;i++){
        text += arr[i] + " ";
    }

    document.getElementById("output").innerText = text;
}
_________________________________________________________________
