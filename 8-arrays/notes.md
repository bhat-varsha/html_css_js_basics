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
🔸 (for arrays)
let fruits = ["apple", "banana"];
for (let fruit of fruits) {
    console.log(fruit);
}
🔸 (for objects)
let person = {name: "Varsha", age: 21};
for (let key in person) {
    console.log(key, person[key]);
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