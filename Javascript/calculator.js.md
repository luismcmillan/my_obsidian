[[Mocking]]
```Javascript
// calculator.js
const math = require('./math');

function calculateTotal(a, b) {
	return math.add(a, b);
}
module.exports = { calculateTotal };
```


```Javascript
// calculator.js
const math = require('./math');

// Original function
function calculateTotal(a, b) {
  return math.add(a, b);
}

// Mocking the add function directly in the code
function mockAdd(a, b) {
  console.log('Mocked add function called');
  return a + b + 1;
}

// Replace the original add function with the mock
math.add = mockAdd;

// Demonstrating the calculateTotal function with the mocked add function
const result = calculateTotal(1, 2);
console.log('Result:', result); // Output should be 4 and log "Mocked add function called"

// If needed, restore the original add function
// Store the original function
const originalAdd = math.add;

// Function to reset the add function to the original implementation
function resetAdd() {
  math.add = originalAdd;
}

// Reset to the original if needed
resetAdd();

// Demonstrate calculateTotal with the original add function
const originalResult = calculateTotal(1, 2);
console.log('Original Result:', originalResult); // Output should be 3

```