Normal javascript is synchronous.

```js
	const name = 'Miriam';
	const greeting = `Hello, my name is ${name}!`;
	console.log(greeting);
	// "Hello, my name is Miriam!"
```
For example, here we expect javascript to first declare a variable name, then the string greeting which uses name, and then log greeting to the javascript console.

It is sequential. 

This code below is also synchronous since the caller has to wait for the function to get executed (at makeGreeting(name))

```js
function makeGreeting(name) {
  return `Hello, my name is ${name}!`;
}

const name = 'Miriam';
const greeting = makeGreeting(name);
console.log(greeting);
// "Hello, my name is Miriam!"

```

However in the same code with a setTimeout function we have an issue. 

```js
	const name = 'Miriam';
	const greeting = `Hello, my name is ${name}!`;
	setTimeout(() => {
		console.log
	}, 8000);
	console.log(greeting);
	// "Hello, my name is Miriam!"
```

Javascript here freezes when it sees the `setTimeout` function and has another handler go ahead an log out `greeting` to the javascript console instead of waiting for `setTimeout()` function to finish. This gives unexpected results. 

Further what if we have a very **long-running synchronous function**:

## Long-Running Synchronous Function:

For the purpose of this example lets say we have a very inefficient 


