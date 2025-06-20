# EP 01

1. Everything in Javascript happens inside an **Execution Context**.
2. it has two components:
   - **Memory Component**: where variables and functions are stored. also called **Variable Environment**.
   - **Code Component**: where the code is executed. also called **Thread of Execution**.
3. Javascript is a **synchronous** **single-threaded** language, meaning it can only execute one task at a time. in specific order.
4. Memory component as contains variables and functions as key-value pairs.
5. Code component as contains the code to be executed in a specific order.

---

**Execution Context Diagram:**

```
+-----------------------------+
|      Execution Context      |
|  +-----------------------+  |
|  |   Memory Component    |  |   <-- Variable Environment
|  |  (Variables, Funcs)   |  |
|  +-----------------------+  |
|  +-----------------------+  |
|  |    Code Component     |  |   <-- Thread of Execution
|  |   (Code Execution)    |  |
|  +-----------------------+  |
+-----------------------------+
```
