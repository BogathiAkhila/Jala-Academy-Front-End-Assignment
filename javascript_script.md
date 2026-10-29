// ==========================================
// 1. JavaScript Basics
// ==========================================

// Single-line comment
/* Multi-line 
   comment block */

let fruits = ["Apple", "Banana", "Mango", "Cherry"];
function sortFruitsDescending() {
    fruits.sort().reverse();
    console.log("Sorted Fruits (Descending):", fruits);
}

const student = { name: "Rahul", role: "Full Stack Developer", batch: "JALA" };
for (let key in student) {
    console.log(`${key}: ${student[key]}`);
}

const person = { firstname: "John", lastname: "Doe" };
console.log("Dot notation:", person.firstname);
console.log("Bracket notation:", person["lastname"]);

hoistedFunction();
function hoistedFunction() {
    console.log("Hoisting demonstration: Functions and var declarations are hoisted.");
}

"use strict";
try {
    // undeclaredVariable = 10; // Throws error in strict mode
} catch (e) {
    console.error("Strict mode caught an error:", e.message);
}


// ==========================================
// 2. JavaScript Access and Properties
// ==========================================

function disappearButton(btn) {
    btn.style.display = "none";
}

function introduce(city, country) {
    return `Hello, I am ${this.name} from ${city}, ${country}.`;
}
const userObj = { name: "Anita" };
console.log(introduce.call(userObj, "Hyderabad", "India"));
console.log(introduce.apply(userObj, ["Hyderabad", "India"]));

let countValue = 0;
function incrementCounter() {
    countValue++;
    console.log("Counter Value:", countValue);
}

const counterObj = {
    _count: 0,
    get count() { return this._count; },
    set count(val) { this._count = val; }
};
counterObj.count = 5;
console.log("Getter Counter:", counterObj.count);

function Vehicle(make) {
    this.make = make;
}
Vehicle.prototype.year = 2026;
const car = new Vehicle("Tesla");
console.log("Prototype Property (year):", car.year);


// ==========================================
// 3. JavaScript Events & Advanced Features
// ==========================================

document.addEventListener("DOMContentLoaded", () => {
    const timeBtn = document.createElement("button");
    timeBtn.innerText = "Show Date & Time";
    timeBtn.onclick = function() {
        alert("Current Date & Time: " + new Date().toLocaleString());
    };
    document.body.appendChild(timeBtn);
});

function validateFormInput(inputField) {
    if (inputField.value.trim() === "") {
        console.warn("Validation error: Field cannot be empty!");
        return false;
    }
    return true;
}

console.log("Debugging checkpoint: Script executed successfully.");

function setCookie(name, value, days) {
    let expires = "";
    if (days) {
        let date = new Date();
        date.setTime(date.getTime() + (days * 24 * 60 * 60 * 1000));
        expires = "; expires=" + date.toUTCString();
    }
    document.cookie = name + "=" + (value || "") + expires + "; path=/";
}

function getCookie(name) {
    let nameEQ = name + "=";
    let ca = document.cookie.split(';');
    for(let i=0; i < ca.length; i++) {
        let c = ca[i].trim();
        if (c.indexOf(nameEQ) == 0) return c.substring(nameEQ.length, c.length);
    }
    return null;
}

function checkCookie() {
    let user = getCookie("username");
    if (user) {
        console.log("Welcome back, " + user);
    } else {
        setCookie("username", "JALA_Student", 30);
        console.log("New cookie set for user.");
    }
}
checkCookie();

const jsonResponse = {
    "status": "success",
    "data": {
        "course": "Full Stack",
        "placementAssurance": 100
    }
};
console.log("JSON Access via Dot Notation - Course:", jsonResponse.data.course);