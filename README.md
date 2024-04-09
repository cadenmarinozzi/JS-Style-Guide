# My Universal JavaScript Style Guide

My style guide rules are simple:

1. Anyone should be able to understand a portion of code, not just the original author.
2. Code should be reusable, readable, and definitive.
3. Code should be as optimized as possible.
4. Each rule should adhere to the other rules.

## Table of Contents

1. [Variables](#variables)

## Variables

- Variables should be singular and represent a single thing.

  - ❌ Bad (Variables represent multiple things):

  ```js
  let names = ["John", "Jane", "Jack"]; // Names is an array of strings representing people.
  names = [20, 25, 30]; // Names now represents something different than the names of people.
  ```

  - ✅ Good (What variables represent doesn't change):

  ```js
  const names = ["John", "Jane", "Jack"];
  const ages = [20, 25, 30];
  ```

- Variables should always be immutable unless they are meant to be changed.
  - ❌ Bad:
  ```js
  let name = "John";
  name = "Jane"; // Name is now Jane.
  ```
  - ✅ Good:
  ```js
  const name = "John";
  const newName = "Jane";
  ```

### Variable names

- Variable names should always be camelCase.

  - ❌ Bad:

  ```js
  const first_name = "John";
  ```

  - ✅ Good:

  ```js
  const firstName = "John";
  ```

- Variable names should always use full words unless they are common abbreviations.

  - ❌ Bad:

  ```js
  const usr = "John";
  ```

  - ✅ Good:

  ```js
  const user = "John";
  ```

  - ❌ Bad (Common abbreviation):

  ```js
  const universalSerialBusNumber = 1;
  ```

  - ✅ Good (Common abbreviation):

  ```js
  const usbNumber = 1;
  ```
