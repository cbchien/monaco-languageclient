# Monaco language client
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://github.com/TypeFox/monaco-languageclient/labels/help%20wanted)
[![Build Status](https://travis-ci.org/TypeFox/monaco-languageclient.svg?branch=master)](https://travis-ci.org/TypeFox/monaco-languageclient)
[![NPM Version](https://img.shields.io/npm/v/monaco-languageclient.svg)](https://www.npmjs.com/package/monaco-languageclient)
[![NPM Download](https://img.shields.io/npm/dt/monaco-languageclient.svg)](https://www.npmjs.com/package/monaco-languageclient)

NPM module to connect Monaco editor with language servers

- Look at [the example client](https://github.com/TypeFox/monaco-languageclient/blob/master/example/src/client.ts) to learn how to start Monaco language client.
- Look at [the example express app](https://github.com/TypeFox/monaco-languageclient/blob/master/example/src/server.ts) to learn how to open a web socket with an express app and launch a language server within the current process or as an external process.

Click [here](http://typefox.io/teaching-the-language-server-protocol-to-microsofts-monaco-editor) for a detail explanation how to connect the Monaco editor to your language server.

Click [here](https://github.com/palantir/python-language-server) for a detail on Python Language Server

## Getting started

```bash
pip install python-language-server
git clone https://github.com/cbchien/monaco-languageclient.git
cd monaco-languageclient
npm install
cd example
npm install
npm run start:ext
```

## Examples

There are two different examples that demonstrate how the `monaco-languageclient` can be used. The Node.js example uses Express and WebSockets to enable communication between the language server process and the web application. The browser example shows how a language service written in JavaScript can be used in a Monaco Editor contained in a simple HTML page.

### Node.js

The example node package is located under the `monaco-languageclient/example` directory. All tasks below should be run from this directory.

From CLI:
- Run `npm install` and `npm run build` to install dependencies and build the example node package.
- Run `npm run start` to start the express server with the language server running in the same process.
- Run `npm run start:ext` to start the express server with language server running in the external process.

After staring the express server go to http://localhost:3000 to open the sample page.

You can as well run vscode tasks to start and debug the server in different modes.

## License
[MIT](https://github.com/TypeFox/monaco-languageclient/blob/master/License.txt)
