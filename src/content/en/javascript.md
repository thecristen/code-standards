## JavaScript

JavaScript is where extra behaviors, features, and functionality not offered natively by Web browsers through CSS and HTML is created. 

### Goals

JavaScript should be used carefully and deliberately. Any and all JavaScript code that's added to a Web page should be there *if and only if* it is necessary for the page to achieve the desired ends.

JavaScript should be:

 - included deliberately, after careful consideration 
 - have the performance overhead and file size evaluated
 - have a feature set that is clearly understood
 - perform only the necessary tasks
 - have maintainability carefully assessed
 - following patterns established for the project
 - tested in various devices and platforms

Likewise, the absense of the code should be carefully considered:

 - What happens if for some reason this code is missing or does not run? 
 - What happens if the code triggers an error?

Please understand what the JavaScript does and how it does it if you are including third party code.

### Getting Started

Client buy-in may be necessary for the usage of JavaScript for various features. It may be a forgone conclusion but usage of libraries or custom code should be discussed with the team and client technical leads for various features.

#### JavaScript Libraries

It is quite common for different libraries and frameworks be used on projects.

#### Have Control Over the Page Lifecycle

 - Single execution and entry point

#### Understanding the Code's Place in the Project

 - Understand where your code will live vs. any code introduced in a destination environment

### JavaScript Standards

#### Inclusion

Use the `<script>` tag to include your JavaScript files at the bottom of your HTML document just before the closing `</body>` tag. For optimal page performance, concatenate your JavaScript into as few files as possible.

```markup
<script type="text/javascript" src="main.js"></script>
```

#### Formatting

The use of whitespace should follow long-standing English writing conventions. Specifically, each comma and colon (and semi-colons that don't end a line) should be followed by a single space. Binary and ternary operators should have a single space on each side. There should be no space characters between parentheses and their contents. Opening braces should appear on the same line as their preceding argument.

```javascript
for (var i = 0, len = arr.length; i < len; i++) {
    // do something
}
```

To maximize readability without worrying about which boolean operators bind more tightly than others, each segment of a boolean expression should be enclosed in parentheses.

```javascript
if ((allowUpdate) && ((user.isAdmin) || (user.role === item.owner))) {
    // do something
}
```

#### Variable Declaration

To avoid confusion between global and local variables, we declare each variable on its own line with the `var` keyword. We do not use a single `var` keyword and then chain several variable declarations onto it separated by a comma.

```javascript
var currentVal = $(this).val();
var min = parseInt($(this).attr('min'), 10);
var max = parseInt($(this).attr('max'), 10);
```

#### Feature Detection

Always test for the existence of a browser API, function, or object property before you use it, and make sure the user experience is still functional (to the extent possible) if it's not found. We rely on JavaScript-based feature detection rather than server-side device detection because it's more robust, easily maintained, and future-proof.

### Deliverables

 - ...

### Next Steps &amp; JavaScript Resources

 - Debugging
 - Patterns for Better JavaScript
 - Unit Testing
 - Node.js

For current links and references, please see our Wiki on Github.
