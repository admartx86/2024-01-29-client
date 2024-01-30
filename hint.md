// script.js

function add(a, b) {
    return a + b;
}

function subtract(a, b) {
    return a - b;
}

function multiply(a, b) {
    return a * b;
}

function divide(a, b) {
    return a / b;
}

module.exports = { add, subtract, multiply, divide };

// script.test.js

const { add, subtract, multiply, divide } = require("./script");

test("adds 1 + 2 to equal 3", () => {
    expect(add(1, 2)).toBe(3);
});

test("subtracts 1 - 2 to equal -1", () => {
    expect(subtract(1, 2)).toBe(-1);
});

test("multiplies 1 * 2 to equal 2", () => {
    expect(multiply(1, 2)).toBe(2);
});

test("divides 1 / 2 to equal 0.5", () => {
    expect(divide(1, 2)).toBe(0.5);
});