# Node.js Cheatsheet

## Overview
- Node.js is an open-source, cross-platform JavaScript runtime environment.
- It is often used for server-side web development, command-line tools, and desktop applications.
- Node.js uses an event-driven, non-blocking I/O model that makes it lightweight and efficient.

## Installation
- Download the Node.js installer from the [Node.js website](https://nodejs.org/en/download/).
- Run the installer and follow the prompts to install Node.js.

## Basic Usage
- Create a new Node.js file with the `.js` file extension.
- Write JavaScript code in the file to perform the desired task.
- Run the file using the `node` command in the terminal.

## Common Modules
- Node.js has a large number of built-in modules that provide useful functionality.
- Some common modules include `http`, `fs`, `path`, and `os`.
- Modules can be imported using the `require` function.

## NPM
- NPM (Node Package Manager) is a package manager for Node.js.
- It allows you to easily install and manage third-party packages.
- NPM packages can be installed using the `npm install` command.

## Example
```javascript
// Example Node.js file
const http = require('http');

const server = http.createServer((req, res) => {
  res.statusCode = 200;
  res.setHeader('Content-Type', 'text/plain');
  res.end('Hello, world!');
});

server.listen(3000, () => {
  console.log('Server running on port 3000');
});
```
This Node.js file creates a simple HTTP server that listens on port 3000 and responds with the message "Hello, world!".

## Resources
- [Node.js Website](https://nodejs.org/)
- [Node.js Documentation](https://nodejs.org/en/docs/)
- [NPM Website](https://www.npmjs.com/)