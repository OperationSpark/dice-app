# Dice App
Build a dice simulator using jQuery.

This entire project should be built using jsbin. When you are done, save your project and send the unique URL to your instructor.

# Part 1: Create the Die

## TODO 1: Create the die element with HTML and CSS

Inside the `<body>`, add a `<div id='die'>` element.

Then, inside the `<head>`, add `<style>` tags and the CSS styles below

```html
<style>
    #die {
        height: 100px;
        width: 100px;
        background-color: lightgray; /* feel free to change this */
        position: relative;
    }
</style>
```

## TODO 2: Import jQuery

Inside the `<head>`, copy-paste the HTML `<script>` tag to import jQuery.

```html
<script src="https://code.jquery.com/jquery-3.5.1.js"></script>
```

## TODO 3: Create a dot in the die with jQuery

_After_ the `<body>`, add a `<script>` tag.

_Inside_ the script tag, use jQuery to create a single dot in the middle of the #die element:

```js
$('<div>')
    .css("height", 15)
    .css("width", 15)
    .css("background-color", "black")
    .css("position", "absolute")
    .css('top', 50)
    .css('left', 50)
    .appendTo("#die");
```  
 
 
# Part 2: Make your code reusable.

## TODO 4: Create a function to make a dot anywhere

Turn your code from TODO 3 into a function that can make a dot in ANY LOCATION. What parameters should this function have? What will change each time you create a new dot?

Name this function `makeDot`.

## TODO 5: Make five dots

Use `makeDot` to create 5 dots on your `#die` element.

# Part 3: Make it random!

## TODO 6: Generate a random number

Use the code below to generate a random number between 1 and 6 each time the program runs:

```js
var randomNum = Math.ceil(Math.random() * 6)
```

## TODO 6: Display the correct number of dots

Use `if` statements to create the correct number of dots based on the random number. Use the image below for guidance.

<img src="/dice.png" width=300>

Your general logic should be:

```
IF randomNum is 1:
	make one dot in the middle
ELSE IF randomNum is 2:
	make two dots in opposite corners
ELSE IF ...
```

## TODO 7: Make it clickable!

Make your die clickable by registering an event handler function to respond to a `"click"` event. Use the general structure below:

```js
// Register an event handler function to be called in response to an "event"
$("element").on("eventType", handlerFn);

// Event handler function
function handlerFn() {

}
```

# Bonus Challenge

Add a second die that would produce a different result from the first.
