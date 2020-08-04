# Dice App
Build a dice simulator using jQuery

# Part 1: Create the Die

## TODO 1: Create the die element with HTML and CSS

Use HTML to create a `<div id='die'>` element inside the `<body>`.

Then, use CSS to style the die with the following properties:

```css
height:100px;
width: 100px;
background-color: your choice
position: relative;
```

## TODO 2: Import jQuery

Copy-paste the HTML `<script>` tag below into your `<head>` to import jQuery.

```html
<script src="https://code.jquery.com/jquery-3.5.1.js"></script>
```

## TODO 3: Create a dot in the die with jQuery

Using jQuery, create a single dot in the middle of the #die element:

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

Call this function `makeDot`.

## TODO 5: Make five dots

Use `makeDot` to create 5 dots on your `#die` element.

SOLVE A NEW PROBLEM
Generate a random number between 1-6:

# Part 3: Make it random!

## TODO 6: Generate a random number

Use the code below to generate a random number each time the program runs:

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

# Bonus Challenge Ideas:

1. Make your die re-roll each time it is clicked. 
2. Have two separate die that can be rolled together
