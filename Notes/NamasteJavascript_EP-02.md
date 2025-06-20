# EP 02

### How JavaScript Code is executed? ❤️& Call Stack

```javascript
var n = 2;
function square(num) {
  var ans = num * num;
  return ans;
}
var square2 = square(n);
var square4 = square(4);
```

1. when the code is executed, it creates an **Execution Context**.
2. In Memory component if it is variable save value as `undefined` and function save as a reference to the function.
3. callstack is created to keep track of the function calls.
4. when the code is executed, it goes through the call stack with global execution context at the bottom.
5. Once the code is completely executed, the call stack is empty.

#### Call Stack maintains the order of execution of execution contexts.

1. Callstack also called as
   - Execution context stack
   - Program stack
   - Control stack
   - Runtime stack
   - Machine stack

---

**Global Execution Context (GEC) - Memory Creation Phase:**

```
Memory Component (Variable Environment)
--------------------------------------
n         : undefined
square    : function reference
square2   : undefined
square4   : undefined
```

**Global Execution Context (GEC) - Code Execution Phase:**

```
Memory Component (Variable Environment)
--------------------------------------
n         : 2
square    : function reference
square2   : 4
square4   : 16
```

**Call Stack:**

```
|----------------------|
|   square(4)          |  <-- Top (last called)
|   square(n)          |
|   Global Context     |  <-- Bottom (first entered)
|----------------------|
```
