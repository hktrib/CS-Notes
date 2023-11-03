Callbacks are functions passed into other functions as arguments to then be called inside the function for some execution

```js
	function greeting(name){
		alert(`Hello, ${name}`);
	}

	function processUserInput(callback){
		const name = prompt("Please enter your name.");
		callback(name);
	}

	processUserInput(greeting);

```

This is a synchronous system, as the callback is executed immediately. Callback's true power is shown with asynchronous systems

