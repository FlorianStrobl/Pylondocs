## JavaScript/TypeScript introduction

JavaScript/TypeScript is a **object oriented programing** (OOP) language, but does this in a different way then most programming languages. It's kinda optional.
In traditional OOP languages, like C++/C# and Java, you have **classes**, were you have your **variables** and **functions**.
```cs
class MyClass { // a class
  int x; // a variable
  
  void MyFunction () { // a function
    // code
  }
}
```
You have e.g. here a class named `MyClass`.
`MyClass` itself has to be instanciated to work. You can think of it like the hardware of a computer. You can buy many computers and they all will have the same parts. A CPU, a GPU, RAM, some drives... but these computers have mostly different CPUs and different sizes of memory aso. They all have the same functionality and use the same parts, but there different.
So, back to programing, all instances of `MyClass` will have a value for `x`, but the value itself may differ from one instance to another. All instances of `MyClass` have here, not just the variable `x`, but also a function called `MyFunction`. You can execut this part of the code whenever you want, but if you use `x` inside the function, it will only use the local value of `x` (the value of `x` setted in **this instance** of `MyClass`).
In some OOP Languages, you have some kind of `Main` class, which has only one instance. So you start from it, and create new instances of other classes in it, and use the variables and functions from these instances.
To say it simple: a class describes an **object** with it's properties in form of **variables** and **functions**.

(Here is one important thing to know if you use Java/C++/C#: there is no global value for `MyClass.x` here, because you don't have a "main instance" of `MyClass`. If you want that all instances of `MyClass` have the same value for `MyClass.x` at all time, you have to make the variable `static`.)

JavaScript/TypeScript is there a bit different. You can have functions **outside** of classes!
Additionaly you can easily say, do function 1 `f1()` but don't wait until it's finish, but do in parallele function 2 `f2()`. 
This is archived with the keyword `async`.
If you have an asynchronous function, but you need it's return value, you have use the keyword `await` to signify that the function should be executed first and after it's completly finished, continue.

// further explanation of TypeScript

## Variables and TypeScripts primitiv types
A variable is pretty much the same thing like in mathematics. You have e.g. an variable named `x` and you can use `x` to perform different actions with it. Unlike mathematics, you know the value of `x` at all points in time.

To create a variable you first need to declare it's name:
```js
let x;
```
If you are using TypeScript, I would hevaly encourage you, to declare it's type too:
```ts
let x: number;
```
After the declaration, you can initzialise it, with it's first value:
```js
x = 5;
```

TypeScript has 12 primitiv types of variables. One important thing to note is: these types are **just for the programer**. The code runs without saying *variable x is from type y* just fine too but it is **way** better do declare it's type. The types are:

**Boolean**: True/False
**Number**: Any number, including negativs and point numbers (in other programing languages often called: floating point number)
**String**: Character**s** including emojis. Strings are written in ""!
**Array**: An array is a list of values. You can have e.g. the array `{0, 5, 1, 7}` which has values from type `Number` in it.
**Tuple**: 
Enum
Any
Null and Undefined
Object
(Void)
(Unknown)
(Never)