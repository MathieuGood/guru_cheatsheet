# JavaScript Cheat Sheet

```js
// Declare variable and constant
let i = 2
let status = false
const message = "hello"

// Declare array
let favoriteMovies = ["Jurassic Park", "Scream", "Alien"]
// Add element at the end of the array
favoriteMovies.push("Dune")
// Delete last element of the array
favoriteMovies.pop()
// Get number of elements in the array
const movieCount = favoriteMovies.length

// Copy by reference value
let a = 1
let b = a
a = 2
// OUPUT : b = 1
// Behaviour with primitive values types (str, bool, number)

// Copy by reference
let a = [1, 2, 3]
let b = a
a.pop()
// OUTPUT : b = [1, 2] = a 
// Behaviour with complex values (function, array, object)

// Do copy by reference value on complex values
let b = [...a]

// Convert variable types
stringToNumber = Number("150")
numberToString = String(150)

// Objets
let computer = {
    brand = "Apple",
    model = "MacBook Pro",
    cores = 12
    ssdGbCapacity = 2048 
}

// Add property to object
client.ramGbCapacity = 32

// Manipulate strings
let sUpper = "HELLO, WORLD!".toLowerCase()
let sLower = "hello, world!".toUpperCase()

// Print in console
console.log(message + " , world!")

// Conditions : if else
if (a === b) {
    console.log("a and b are equal")
} else {
    console.log("a and b are different")
}

// Conditions : switch case
switch (dayName) {
    case "Monday":
    case "Tuesday":
    case "Wednesday":
    case "Thursday":
    case "Friday":
        console.log("Week")
        break
    case "Saturday":
    case "Sunday":
        console.log("Weekend")
        break
    default:
        console.log("Not a valid day name")
}

// For loop
for (let i = 0; i < 3; i++) {
    console.log(i)
}

// While loop
let i = 0
while (i < 3) {
    console.log(i)
    i++
}

// Function
function returnWelcomeMsg(name, city) {
    let msg = "Hello " + name + ", welcome to " + city
    return msg
}

```

```html
<!DOCTYPE HTML>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Web page example</title>
    <link rel="stylesheet" href="style.css">
    <!-- Link js files -->
    <!-- 'defer' option delays the execution of the scripts until all scripts are loaded -->
    <script src="scripts/config.js" defer></script>
    <script src="scripts/main.js" defer></script>
</head>

<body>
    <header>
        <h1>Typing test</h1>
    </header>
    <main>
        <div id="wordToTypeZone">
            <span>Enter your text :</span>
        </div>
    </main>
</body>

</html>


```

