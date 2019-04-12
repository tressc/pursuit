#### Variable Exercise 1:

With you partner, predict what you'll see in the REPL when you run each line in the following code. If you're not sure or can't agree, run the line in question and then discuss.

```js
> var myVar

> myVar // A: what is the value of myVar now?

> myVar = 5

> myVar // B: what is the value of myVar now?

> myVar + 2 // C: what does this evaluate to?

> myVar // D: what is the value of myVar now?

> var myOtherVar = 10

> myOtherVar // E: what is the value of myOtherVar
```

#### Variable Exercise Part 2:

Past the following code snippets into a JS file. With your partner, try to predict what will the `console.log`s will print out . Then run the code and compare the result to your predictions.

If you missed any, discuss with your partner, and see if you can figure out what the code is doing. If you get stuck, ask your instructor to come over!

A great way to get more comfortable with variables is to make changes in the examples below and see how what gets printed out changes. Small changes can have big consequences, which is part of what makes programming so powerful!

```js
// 1
var idx = 'abcde'.indexOf('D');
idx = idx + 11;
console.log(idx); // ?
idx * 2;
console.log(idx); // ?
```

```js
// 2
var num = 33;
var isEven = num % 2 === 0;
console.log(isEven); // ?
var isOdd = !isEven;
console.log(!isOdd); // ?
```

```js
// 3
var str1 = 'marker';
var num = 'whiteboard'.length - str1.length;
console.log(num); // ?
var str2 = 'pursuit';
console.log(str2[num].toUpperCase()); // ?
var char = str2[num].toLowerCase(); // ?
console.log(char + '!'); // ?
```

```js
// 4
var sentence = 'it was a dark and stormy night';
var lastChar = sentence[sentence.length - 1];
console.log(lastChar); // ?
console.log(sentence.indexOf(lastChar)); // ?
```

#### (Bonus) Variable Exercise 3

Past the following code snippets into a JS file. With your partner, declare the necessary variables and assign them values so that the code prints out the message at the bottom.

```js
// 1
var message = greeting + " " + name;
var excited = message.toUpperCase() + "!!!";
console.log(excited) //=> "OH HI MARK!!!"
```

```js
// 2
var c = a + b;
var d = c / 3;
console.log(d) //=> 6
```

```js
// 3
var percent = (tip / mealCost) * 100
var isReallyBigTip = percent > 50;
console.log(isReallyBigTip) //=> true
```
