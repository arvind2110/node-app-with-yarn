# Setup Node application using YARN and TypeScript
* Setting up a Node.js project using Yarn is a straightforward process. Yarn is a popular package manager for Node.js projects that offers various advantages over npm.
* Here's a step-by-step guide to help you set up a Node.js project using Yarn:
* * Prerequisites: 
* * * Install Node.js(https://nodejs.org) and Yarn
* * * * Yarn installed globally. You can install Yarn using npm with the following command: 
* * * * * ``` npm install -g yarn ```
* * Create a new project directory
* * Initialize the project:
* * * ``` yarn init -y ```
* * Install dependencies:
* * * yarn add express @types/express typescript ts-node
* * * * express: This package is used to create the HTTP server.
* * * * @types/express: This package contains TypeScript type definitions for Express to enable type checking.
* * * * typescript: This is the TypeScript compiler.
* * * * ts-node: This allows you to run TypeScript files directly without the need to compile them first.
* * Create a TypeScript configuration file:
* * * Create a tsconfig.json file in the root of your project. This file will contain the configuration for the TypeScript compiler. You can create it manually or use TypeScript's CLI to generate it:
* * * * ``` npx tsc --init ```
* * * * * This will create a tsconfig.json file with default settings. You can customize it according to your project's needs.
* * Create the source code directory and server file:
* * * Create a new directory named src in your project's root folder. Inside the src directory, create a file named server.ts. This file will contain the code for your HTTP server.
* * Update package.json to run the server using ts-node:
* * * In the scripts section of your package.json file, add a script to run the server using ts-node:
* * * * ``` "scripts": { "start": "ts-node src/server.ts" } ```
* * Start the server:
* * * ``` yarn start ```