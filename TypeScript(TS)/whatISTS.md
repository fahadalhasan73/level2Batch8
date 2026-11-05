TypeScript (TS) is a programming language developed by Microsoft that builds on JavaScript (JS) by adding features such as static typing, better error detection, and improved code organization.

In simple words:

TypeScript = JavaScript + Type Safety + Additional Developer Features

TypeScript is especially useful for developing large websites, web applications, and backend systems.

## 1. JavaScript vs TypeScript  
Suppose we're creating a function that adds two numbers.
```powershell

function add(a, b) {
  return a + b;
}

console.log(add(10, 20));    // 30
console.log(add("10", 20));  // "1020"
  
```
JavaScript allows us to pass a string instead of a number. This can produce unexpected results.  
""TypeScript""

```powershell

function add(a: number, b: number): number {
  return a + b;
}

console.log(add(10, 20));    // 30
console.log(add("10", 20));  // Type error
  
```
TypeScript detects the incorrect argument during type checking, before the program runs.