Challenge: Implement a Debounce Function
Objective: Implement a debounce function that delays the processing of the input function until after a specified wait time has passed since the last time the debounce function was invoked.

Instructions:

Debounce Function Signature: Create a function debounce that takes two arguments:
func (Function): The function to debounce.
wait (Number): The number of milliseconds to delay.

Functionality:
The debounce function returns a new function that, when executed, delays the invocation of func until after wait milliseconds have elapsed since the last time the returned function was invoked.

Example:
```javascript
function sayHello() {
  console.log('Hello!');
}

const debouncedSayHello = debounce(sayHello, 2000);

debouncedSayHello(); // Will not log 'Hello!' immediately
debouncedSayHello(); // Resets the timer, will log 'Hello!' 2 seconds after this call
```

Hints:
Use setTimeout to delay the execution of the function.
Use clearTimeout to reset the delay if the returned function is called again before the wait period is over.
