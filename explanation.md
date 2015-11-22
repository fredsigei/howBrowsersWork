<h1><b>Simple explanantion on how browsers work</b></h1>

Browser is a program with a graphical user interface for displaying HTML files, its uasualy used to navigate the www
 
The browser's main functionality

The main function of a browser is to present the web resource you choose, by requesting it from the server and displaying it in the browser window. The resource is usually an HTML document, but may also be a PDF, image, 
or some other type of content. The location of the resource is specified by the user using a Uniform Resource Identifier.

The way the browser interprets and displays HTML files is specified in the HTML and CSS specifications. These specifications are maintained by the W3C (World Wide Web Consortium) organization, which is the standards 
organization for the web.

Browser user interfaces have a lot in common with each other. Among the common user interface elements are:

1) Address bar for inserting a URI
2) Back and forward buttons
3) Bookmarking options
4) Refresh and stop buttons for refreshing or stopping the loading of current documents
5) Home button that takes you to your home page

 The HTML5 specification doesn't define UI elements a browser must have, but lists some common elements. Among those are the address bar, status bar and tool bar. There are, of course, features unique to a specific browser like
 Firefox's downloads manager.

The browser's main components are 

The user interface
This includes the address bar, back/forward button, bookmarking menu, etc. Every part of the browser display except the window where you see the requested page.

The browser engine
This marshals actions between the UI and the rendering engine.

The rendering engine
This is responsible for displaying requested content. For example if the requested content is HTML, the rendering engine parses HTML and CSS, and displays the parsed content on the screen.

Networking
For network calls such as HTTP requests, using different implementations for different platform behind a platform-independent interface.

UI backend
Is used for drawing basic widgets like combo boxes and windows. This backend exposes a generic interface that is not platform specific. Underneath it uses operating system user interface methods.

JavaScript interpreter
Is Used to parse and execute JavaScript code.

Data storage. 
This is a persistence layer. The browser may need to save all sorts of data locally, such as cookies. Browsers also support storage mechanisms such as localStorage, IndexedDB, WebSQL and FileSystem.

Browsers such as Chrome run multiple instances of the rendering engine: one for each tab. Each tab runs in a separate process

The rendering engine
The responsibility of the rendering engine is to display the requested contents on the browser screen.
By default the rendering engine can display HTML and XML documents and images. It can display other types of data via plug-ins or extension; for example, displaying PDF documents using a PDF viewer plug-in.

Rendering engines
Different browsers use different rendering engines: Internet Explorer uses Trident, Firefox uses Gecko, Safari uses WebKit. Chrome and Opera (from version 15) use Blink, a fork of WebKit.
WebKit is an open source rendering engine which started as an engine for the Linux platform and was modified by Apple to support Mac and Windows. See webkit.org for more details.

The main flow
The rendering engine will start getting the contents of the requested document from the networking layer. This will usually be done in 8kB chunks.

 Rendering engine basic flow
The rendering engine will start parsing the HTML document and convert elements to DOM nodes in a tree called the "content tree". The engine will parse the style data, both in external CSS files and in style elements. 

