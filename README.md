# Budget Calculator

## Project Creation

- Create a Project :beers:.
- ```bash
  npx degit sveltejs/template budget-calculator
  ```
- ```bash
  npm i
  ```
- ```bash
  git init
  ```
- Create a repository in github.
- Copy this below command and paste in VS code terminal
  ```bash
  git remote add origin https://github.com/SanthoshRaghav/budget-calculator.git
  ```
- ```bash
  npm add .
  ```
- ```bash
  npm commit -m "initial commit"
  ```
- ```bash
  git push -u origin master
  ```

## New Things to Remember

1. How to make "component spefic Css properties" to "global Css properties"

   ```css
   :global(span) {
     background: teal;
     color: white;
   }
   *parenthesescancontain: -(element, classsname, id);
   ```

2. Importing a JS file, suppose if you are importing a " js file ", then it does't requre a file extension.
   ```js
   import expensesData from "expenses";
   ```
3. import statements from ES6

   1. importing a component with in the current folder.

   ```js
   import component from "./component.svelte";
   ```

   2. importing a component outside the current folder.

   ```js
   import component from "../component.svelte";
   ```

   3. importing a "packages" from node modules folder.

   ```js
   import package from "packageName";
   ```

   4. Don't import props using const keyword :beetle: use "let" keyword

   ```js
   export const title = "Default title";
   ```

4. Ways to send props

   ![Drag Racing](./public/images/expense.png)

   1. Sending props normally....

      ![Drag Racing](./public/images/sending-props-normally.png)

      #### we can receive props two ways...

      1. Normal way...

         ![Drag Racing](./public/images/normal.png)

      1. Destructing way...

         ![Drag Racing](./public/images/destructing.png)

   2. Spreading props and sending....

      ![Drag Racing](./public/images/spreading-and-sending-props.png)

      1. Receiving way...

         ![Drag Racing](./public/images/spreading-and-sending-props-and-receiving.png)

5. Sending function as a prop (Parent to child)

   1. Parent Component

      ![Drag Racing](./public/images/spreading-and-sending-props-and-receiving.png)

   2. Child Component (ExpenseList.svelte component)

      ![Drag Racing](./public/images/sending-function-as-a-prop-in-Expense-and-calling.png)

   3. Child Component (Expense.svelte component)

      ![Drag Racing](./public/images/sending-function-as-a-prop-in-Expense-and-calling.png)

6. Context API

   1. setContext

      ![Drag Racing](./public/images/setcontext.png)

   1. getContext

      ![Drag Racing](./public/images/getcontext.png)
