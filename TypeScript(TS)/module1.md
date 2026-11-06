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


## Why do we need JavaScript?
Let's consider the following JS code
```powershell
const addTwo = (a,b) => {
  return a+b
}
console.log (addTwo("10", 20))
const user = {
  name: "Fahad Al Hasan"
}
console.log (user.name)
console.log (user.address)
console.log (user.address.city)
```
**Output**
```powershell
1020
Fahad Al Hasan 
undefined 
ERROR! 
/tmp/UWrlrihR6U-IbhuUBBW/main.js:10
console.log (user.address.city)
                          ^

TypeError: Cannot read properties of undefined (reading 'city')
    at Object.<anonymous> (/tmp/UWrlrihR6U-IbhuUBBW/main.js:10:27)
    at Module._compile (node:internal/modules/cjs/loader:1781:14)
    at Object..js (node:internal/modules/cjs/loader:1913:10)
    at Module.load (node:internal/modules/cjs/loader:1505:32)
    at Function._load (node:internal/modules/cjs/loader:1309:12)
    at wrapModuleLoad (node:internal/modules/cjs/loader:254:19)
    at Function.executeUserEntryPoint [as runMain] (node:internal/modules/run_main:171:5)
    at node:internal/main/run_main_module:36:49

Node.js v22.23.4
```
**Output Explanation:**  
JavaScript Coercion: When the type of two value are different then JS tries to convert same type by force.
```
console.log (addTwo("10", 20)
```
Here JS making 20 as string by force. That's why concatenation happens and the output is  **1020**  
["10" + "20"] This is occurring here actually  

At next, When we are trying to access the address property of the user, then there is nothing namely address and the output is simply undefined. But after that when we are trying to accessing a nested property then **ERROR!** comes. Because address doesn't have any existence then how something inside address can be accessed?  
That's why JS is giving the **TypeError.**  

The reason is - JS is dynamic type programming language.  
There is no fix type are there for variable. JS give some types to the variables during runtime which is unexpected.  
JavaScript is compiled line by line - Interpretation.  
JIT [Just In Time] Compiler  
The type errors can't be solved during development. This comes front after running. This is problem. 


**Static Typed Programming Language**  [C#]  
**Dynamic Typed Programming Language** [JavaScript]
<br> <br> <br>
<img width="1111" height="485" alt="image" src="https://github.com/user-attachments/assets/292b955d-2efd-461c-b657-d685a61c83ce" />
<br> <br> <br>
## Program Flow  
<img width="1366" height="944" alt="image" src="https://github.com/user-attachments/assets/65c569d6-a4af-47ad-b166-cd17c5a6f4b6" />

## Development Environment Setup


