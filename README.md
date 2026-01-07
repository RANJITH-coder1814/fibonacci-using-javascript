# fibonacci-using-javascript

This project demonstrates how to generate the Fibonacci sequence using JavaScript.

## 📌 What is Fibonacci Series?
The Fibonacci series is a sequence of numbers where:
- The first number is 0
- The second number is 1
- Each subsequent number is the sum of the previous two numbers

Example:
0, 1, 1, 2, 3, 5, 8, ...

## 💻 JavaScript Code

```javascript
function fibonacciGenerator(n) {
    let output = [];

    if (n === 1) {
        output = [0];
    } else if (n === 2) {
        output = [0, 1];
    } else {
        output = [0, 1];
        for (let i = 2; i < n; i++) {
            output.push(output[i - 1] + output[i - 2]);
        }
    }

    return output;
}

let result = fibonacciGenerator(5);
console.log(result);

