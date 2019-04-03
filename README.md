# typescript-crash-course
A learning repo for typescript

## What's TypeScript?
  * An open-sourced, syntatic superset of JavaScript, developed by MS. 
  * Compiles to readable JavaScript. 
  * Comes with three parts: Language, Language Server, and Compiler. 
  * Works well with Babel 7 
## Rationale behind types
  * Encode constraints and assumptions, such as input sanitation
  * Catch common mistaktes (i.e. incomplete refactors) 
  * Move some runtime errors to compile time (earlier feedbacks, as opposed to learning of mistakes at runtime)
  * Provide consumers (including you) with a great DX (design experience)

## TypeScript Compiler 
 ### Manual Compiler setup
  * To compile typescript files run 
    ```tsc filename.ts --target ES2017 --module commonjs --watch``` in the terminal.
  * To open up the compiled code run  `code filename.js` in the terminal.
 ### Automated Setup
  * To configure the tsc command to compile without the additional flags, create a tsconfig.json file.
  * Set up the file as follows: 
    ```
      {
        "compilerOptions": {
          "module": "commonjs", 
          "target": "ES2017",
          "outDir": "lib"
        },
        "include": ["src", "tsconfig.json"]
      } 
    ```
