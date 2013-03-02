#Using the Interface.js Editor

NOTE: Until binaries are distributed using this software requires basic knowledge of node.js and npm.

![Screenshot](https://raw.github.com/charlieroberts/interface.editor/screenshots/editor_screenshot.png) 

This project is a WYSIWYG editor for creating interfaces using [Interface.js][interfacejs]. When used in conjunction with the [Interface.js Server project][interfaceserver], these interfaces can transmit OSC or MIDI messages from (almost) any web browser, including those found on mobile devices such as mobile Safari, Chrome and mobile Firefox. Although you can program interfaces for Interface.js using JavaScript, this editor provides drag and drop controls for placing widgets and defining their properties.
  
The editor will eventually be distributed as a compiled binary application for OS X, Linux and Windows, but for now if you want to use the editor you'll need to download and install [node.js][nodejs]. Node.js will provide most of the functionality we need to serve web pages, but we'll also need to add a few utility libraries to send OSC and MIDI and carry out a few other specialized tasks. We can install these utilities using the [Node Package Manager][npm], or NPM, which is installed with Node.js. After installing Node.js, open a terminal and run the following commands:

```
npm install midi
npm install omgosc
npm install connect
npm install ws
```

The last step is to download [node-webkit][node-webkit]. Node-webkit enables desktop applications to be built using web technologies. Once you have Node-webkit installed, place this directory in the same location. You can then open the editor as follows:

```
./nw projectDirectoryName
```

[nodejs]:http://nodejs.org
[npm]:http://nodejs.org/download/
[node-webkit]:https://github.com/rogerwang/node-webkit
[interfacejs]:https://github.com/charlieroberts/interface.js
[interfaceserver]:https://github.com/charlieroberts/interface.server
