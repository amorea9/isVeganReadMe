# A short guide for _"is-vegan"_: an npm module

##

### It's friday evening and your friends are coming over for dinner.

### All of a sudden you realise one very important thing.. something you hadn't thought about before... something that could change everything... your friends are _vegan_ and you are not.

### You have 0 experience with vegan cusine and definitely don't want to f\*\*\* up, cooking something that you thought was vegan but it's not...

### If this is you.. well first of all don't panic, it's not too late!

### Open up your laptop, run VS code and I'll explain the rest.

<br>

# What it does

##

### _"is-vegan"_ is an npm module that can identify if an ingredient is vegan or not by going through specific databases.

### It is incredibly useful if you have no internet to google and have a laptop to use.

<br>

# How it works

##

### First of all, I hope you're ready for this, have your laptop on, VScode running and a test project set up.

### If you are, you can then easily follow these steps:

<br>

- open the terminal and type in <br> <pre><code>"npm install is-vegan --save"</code></pre>

  <br>

- after that's installed, make sure to run the commands<pre><code>npm run build</code> and <code>npm run dev</code></pre> so that you can access the live server and console.

<br>

- import the module in your javascript file<pre><code>import \* as isVegan from "is-vegan"; </code></pre>

<br>

### We are now ready to test it out!

### Let's head to our javascript file again!

<br>

- we will check if a specific ingredient is vegan by typing: <pre><code>console.log("Is salmon vegan?", isVegan.isVeganIngredient("salmon"));</code></pre>

<br>

- in our console, the result will be shown just like this: <pre><code>Is salmon vegan? False </code></pre>

### We can also give it a list of ingredients and make it check if it is vegan friendly or not. Or we can think in reverse and ask it which specific ingredients are not vegan.

### An example below:

- In javascript:
<pre><code>// example 1 - to check if the ingredients are vegan friendly. If at least one ingredient is not vegan, it returns false.

console.log("Is it vegan friendly?", isVegan.isVeganIngredientList(["salmon", "cheese", "butter", "tofu", "sugar"]));

//example 2 - to check which specific ingredients are not vegan

console.log("What is non vegan?", isVegan.containsNonVeganIngredients(["salmon", "cheese", "butter", "beef", "sugar"]));
</code></pre>

- in the console
<pre><code>// example 1 result (boolean)
Is it vegan friendly? false

//example 2 result (array)

What is non vegan?
Array(4) [ "salmon", "cheese", "butter", "beef" ]
</code></pre>

<br>

# Conclusion

##

### To conclude:

- you get to use a cool little tool
- your friendship is saved
- I am done with my assignment

### _You're welcome!_

<br>

If you want to read more you can head to _is-vegan_ [npm page](https://www.npmjs.com/package/is-vegan)
