# calculator-react
A simple calculator application using JavaScript library React JS

![Calculator Image](https://image.ibb.co/cT0CAa/calculator.jpg)


##Information
* Two react objects Square and Board are created. Square renders a square with a props 'number'. Board renders number of squares(In my case 16 squares)

* `var lastCharacter = txtString.value.substr(txtString.value.length - 1);` This assigns previous character to the variable lastCharacter.

* `if (lastCharacter<'0' || lastCharacter>'9')` This condition is to check whether last character is numeric or not.

* `if (this.props.number<'0' || this.props.number>'9')` This condition is to check whether currently entered character is numeric or not.

* If two symbols(non numeric characters) entered together, It prevents lastone from appending in the textbox. and, Initially anything other than numbers are restricted to enter.

* `txtString.value+=this.props.number;` This apppends currentle pressed value to the existing value of the textbox.

* `result= eval(txtString.value);` Here, eval is a builtin js function, it does maths operation on well formatted combination of numeric and symbols.so, we have tried to avoid all unexpected characters from above to make string acceptable for `eval` function.

* `txtString.focus();` It is kept to return focus to the textbox immediately after pressed the button.

##Dependencies needed
`react.js` and `react-dom.js` are included in js folder. `browser.min.js` is to run JSX, CDN is included.

##Demo
http://psuresh.com.np/Miscellaneous/calculator
