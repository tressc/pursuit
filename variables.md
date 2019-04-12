### Variables:

All the work we've done in a REPL up to this point has kind of been like using a handheld calculator. We can do one operation, but as soon as we do a second, the old result is gone. That's not very useful, so we need a way to store information over time!

#### Variables to the rescue!

Variables are like labeled boxes with information inside. We can create variables like this:

#### Variable Declaration

```js
var myNum;

console.log(myNum) //=> undefined
```

**Notice** what happens if we try to `console.log` a variable name that doesn't exist!

We use the `var` keyword to introduce (**declare**) a variable name (the labeled box) to our code. Now whenever we use that name, JavaScript with give us the value stored inside.

Notice how we get `undefined` if we ask JS for the value of `myNum`. That's because there's no value in there yet. Let's add that now:

#### Variable Assignment:

```js
myNum = 9;

console.log(myNum) //=> 9
```


Here we use the single equals `=` *assignment operator* to put a value "inside" (**assign**) `myNum`. If we access `myNum` now, we get back `9`.

We can do **declaration** and **assignment** all at the same time on one line:

```js
var myName = "colin";

console.log(myName) //=> colin
```

Notice that we only use var the first time we introduce the new variable!

*Try making some variables in the REPL*

We can also change out the value in a variable at a later time:

#### Variable Re-assignment

```js
var currentYear = 2018;
currentYear = 2019;

console.log(currentYear)
```

To *re-assign* a variable, we must use the assignment operator. `var` is no longer necessary.

#### Exercise 1

Pause here and do [exercise 1](./exercises.md).

#### Helpful Re-assignment Tricks

In **exercise 1** we saw that `myVar + 2` evaluated to `7`, but it didn't actually update the value of `myVar`. If we want to reassign myVar to this new value, there's a few ways we can write it:

```js
var myVar = 5;

console.log(myVar); // 5

myVar = myVar + 2; // notice the single equals!

console.log(myVar); // 7

// we can also write this same expression in a faster way
myVar += 2;

console.log(myVar); // 9

// if we only want to add 1, we can also write:
myVar++;

console.log(myVar); // 10
```

Available operators are `+=`, `-=`, `*=`, `/=`, `%=`, `++`, and `--`.

#### Exercises 2 & 3

Pause here and do [exercises 2 & 3](./exercises.md#variable-exercise-2).

#### Good Variable Names

There are only a few strict rules we need to follow when naming variables. Beyond those rules are a number of conventions for making our code readable and easy to understand.

**Rules:**

Variable names can only contain:
  - letters
  - numbers
  - underscores
  - dollar signs

Variable names can *never start with a number.*
  - better: `var twenty_20$Dollars = 20`
  - worse: `var 20-twenty.dollars = 20`

*In a REPL, test out what happens when you declare the "worse" variable above.*

**Conventions:**

Variable names:
  - are written in camelCase
    - better: `var thisNameIsInCamelCase = "hello"`
    - worse: `var this_one_is_not = "hello"`
  - are short but descriptive
    - better: `var smallNumber = 15`
    - worse: `var x = 15`
    - worse: `var aReallySmallNumberIMeanSuperSmall = .00002`

*In a REPL, test out what happens when you declare the "worse" variables above.*
