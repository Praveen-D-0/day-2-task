

# Quesiton 1
## The Differences Between the Document and Window Objects



A document is an object inside the window object and we use a document object for manipulation inside the document.

The first thing that gets loaded into the browser is the window and the properties related to that window are stored in the window object. Properties related to window objects are length, innerWidth, innerHeight, caches, etc.

There was a document object too so what about it then?

So after the window gets loaded then there’s a document (HTML, PHP, or another document) loaded inside that window, and the properties related to that document is stored in the document object. Properties related to document objects are title, URL, cookie, etc.

The window is at a root/top level at the JavaScript object hierarchy. It  is a global/root object in JavaScript and it is the root object of the Document object model(DOM);


In the world of web development, understanding the intricacies of the Document and Window objects is like unlocking the keys to a vast kingdom of dynamic and interactive web experiences. These objects are at the core of the Document Object Model (DOM), a critical concept that governs how web pages are structured, manipulated, and interacted with. Let's dive into the differences between the Document and Window objects and explore their roles in shaping the modern web.

###  Introduction to the Document and Window Objects

The Document and Window objects are essential components of the DOM, a programming interface that represents the structure of an HTML document as a tree of objects. The DOM enables developers to access and manipulate elements on a web page dynamically.

The Document object represents the entire HTML document and provides methods and properties for interacting with the contents of the document, such as selecting elements, modifying attributes, and manipulating the structure.

The Window object, on the other hand, represents the browser window or tab that contains the document. It acts as a global object, providing methods and properties for managing the browser window, controlling navigation, and interacting with the user.

###  Scope and Access

The Document object is tightly coupled with the current web page. It primarily deals with the structure and content of the HTML document. You can access elements using methods like `getElementById()`, `querySelector()`, and more. The Document object provides properties and methods for managing the content within the document, such as `createElement()`, `appendChild()`, and `innerHTML`.

The Window object is a broader entity that encompasses the entire browser window or tab. It provides access to global properties like `location`, `navigator`, and `history`. The Window object also allows you to control the behavior of the browser, open new windows or tabs using `window.open()`, and manipulate the dimensions of the current window.

###  Methods and Properties

The Document object focuses on methods and properties for interacting with HTML elements. For instance, you can use `getElementById("elementId")` to retrieve an element by its ID or `querySelector(".classname")` to select elements using CSS selectors. The Document object also provides properties like `body`, `title`, and `URL` to access specific parts of the document.

The Window object concentrates on methods and properties related to the browser window. You can use `window.alert()`, `window.confirm()`, and `window.prompt()` for interacting with the user. The Window object also provides properties like `window.innerWidth`, `window.innerHeight`, and `window.location` to manage the window's dimensions and navigation.

### The Differences Between the Document and Window are:

|               Document                                              |              Window                                             | 
|---------------------------------------------------------------------|-----------------------------------------------------------------|
|It represents the document loaded inside the window or browser.	    | It represents the browser window in which you are seeing the content.|
|The properties related to it are stored in the document object.	    | The properties related to it are stored in the window object.    |
|It is loaded after the loading window because the window contains a document.|	It is loaded before the document because window container document |
|It is the root element of the document object model.                 |	The window is the global element for all objects, functions, etc.|
|We can not access windows objects properties inside the document.    |	We can access document object properties inside the window.      |
|logically:                                                           |logically: 
           document:{ properties}                                                 window:{ 
                                                                                     document:{properties} 
                                                                                     }                                                           |
|Example: document.title will return the title of the document        |	Example: window.document.title will return the title of the document. |

In the dynamic landscape of web development, the Document and Window objects hold pivotal roles in shaping how users interact with web pages and how developers create rich and engaging experiences. Understanding the distinctions between these two objects empowers developers to harness the power of the DOM and create web applications that are responsive, interactive, and user-friendly. Whether you're manipulating the content within a document or controlling the behavior of the browser window, the Document and Window objects are your allies in crafting the next generation of web experiences.
