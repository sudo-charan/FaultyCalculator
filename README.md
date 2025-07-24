# ⚠️ Faulty Calculator 🤖

This is a fun and simple **"Faulty Calculator"** built using HTML and JavaScript. It looks like a regular calculator, but with a twist — sometimes it gives *intentionally wrong answers* just to mess with you.

---

## 🚀 How It Works

- User is prompted to enter:
  - First number
  - Operator (`+`, `-`, `*`, `/`)
  - Second number
- In **90%** of cases, it gives the **correct result**.
- In **10%** of cases, it purposely **swaps the operator** and gives a **wrong result**.
  
For example:
- Input: `3 + 5`  
- Possible Faulty Output: `3 - 5 = -2` (instead of `8`)

---

## 🤖 Fault Logic

The operator is randomly swapped based on a small chance using this mapping:

```js
{
  "+": "-",
  "*": "+",
  "-": "/",
  "/": "**"
}
