[[Mocking]]
```Javascript
// calculator.test.js
const calculator = require('./calculator');
const math = require('./math');
// Mock the add function
jest.mock('./math');
test('calculateTotal uses math.add', () => {
	// Arrange
	math.add.mockImplementation((a, b) => a + b);
	// Act
	const result = calculator.calculateTotal(1, 2);  
	// Assert
	expect(result).toBe(3);
	expect(math.add).toHaveBeenCalledWith(1, 2);
});
```