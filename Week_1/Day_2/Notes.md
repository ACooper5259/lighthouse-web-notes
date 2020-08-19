# Day 2 Notes

## Functions

Naming:
* avoid generic names like 'data', or 'run'
* name your functions beginning with action words like createUser, or sendUserData
* be consistent with your naming conventions
* if you're joining an existing project, observe and adapt any existing conventions

A JavaScript Specific Naming Convention: use camelCase

Functions should focus on a single task: returning a value or causing a side effect. Break your function into additional smaller functions if you find it doing two or more things

## Truthy and falsey
In JS, everything has an inherent Boolean value, which is commonly referred to as a Truthy or Falsey value. In this case, even though 0 is a Number, it also holds a Falsey value.
Most things in JavaScript are considered Truthy, except for the following:
* false
* 0
* null
* undefined
* NaN

Truthy values are a fast and easy way to check conditions in our code. For example, maybe we want to save the users name to a String, but only if we don't already have something saved to username.

```
username = '';
//if username is falsy, ie empty
if (!username) {
  username = 'Siobhan';
}
```
The same concept can be applied to Arrays. Invoking the Array.length property will return 0 for an empty Array, which is also a falsey value.
```
shoppingList = [];

if (!shoppingList.length) {
  shoppingList.push('coconut milk');
}
```