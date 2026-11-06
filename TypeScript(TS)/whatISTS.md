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
```
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

<table>
<tr>
<td>

**Output**

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

</td>
</tr>
</table>



**Static Typed Programming Language**  
**Dynamic Typed Programming Language**