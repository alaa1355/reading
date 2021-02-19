### Syntax Errors

Syntax errors are the most common type of error that occurs in any programming language. As the name suggests, something incorrect in the syntax of the program body raises this error. Syntax errors are also known as  **parsing errors**. In JavaScript, they occur at the interpretation time.

Consider this code segment:

1.   \&lt;script type=&#39;&#39;text/javascript&#39;&#39;\&gt;
2.     window.show(;
3.   \&lt;/script\&gt;

This program will raise an error as the closing bracket of the show function is missing.

### Runtime Errors

These type of error occurs during the runtime of the program, after it is interpreted by the compiler.

Consider this code segment:

1.   \&lt;script type=&#39;&#39;text/javascript&#39;&#39;\&gt;
2.     window.show();
3.   \&lt;/script\&gt;

Notice that there is no show function defined. This program will raise an error at runtime as the function which is not present is called, although the syntax is correct.

### Logical Errors

These type of errors are the most difficult to find. Consider a statement: &#39;&#39;John is playing guitar.&#39;&#39; This statement is logically correct and its syntax is also correct. Now consider another statement: &#39;&#39;Guitar is playing John.&#39;&#39; This statement is correct with respect to its syntax but is logically incorrect. These types of errors cause a serious problem as they change the whole path of how your program will work.

## Methods to Prevent Errors

### Onerror() Method

In this method, an  **error event**  is fired when an error occurs. This method also works for those errors caused by external sources. Whenever an error is caught, this method tells the developer the line number at which the error has occurred, the file to which the error has occurred and displays a customized error message.

Consider the following code segment:

1.   \&lt;html\&gt;
2.   \&lt;head\&gt;
3.   \&lt;script type=&#39;&#39;text/javascript&#39;&#39;\&gt;
4.     window.onerror = function (){
5.     alert(&#39;&#39;An error has occurred.Please resolve&#39;&#39;);
6.     }
7.   \&lt;/script\&gt;
8.   \&lt;/head\&gt;
9.   \&lt;body\&gt;
10.   \&lt;p\&gt;Click to see the result:\&lt;/p\&gt;
11.   \&lt;form\&gt;
12.   \&lt;input type =&#39;button&#39; value =&#39;Click&#39; onclick =&#39;myFunc();&#39;/\&gt;
13.   \&lt;/form\&gt;
14.   \&lt;/body\&gt;
15.   \&lt;/html\&gt;

When the button is clicked, the error message &#39;&#39;An error has occurred. Please resolve&#39;&#39; is displayed.

**TypeError**

The  **TypeError**  object represents an error when an operation could not be performed, typically (but not exclusively) when a value is not of the expected type.

A TypeError may be thrown when:

- an operand or argument passed to a function is incompatible with the type expected by that operator or function; or
- when attempting to modify a value that cannot be changed; or
- when attempting to use a value in an inappropriate way.

The  **RangeError**  object indicates an error when a value is not in the set or range of allowed values.

## [Description](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/RangeError#description)

A RangeError is thrown when trying to pass a value as an argument to a function that does not allow a range that includes the value.

This can be encountered when:

- passing a value that is not one of the allowed string values to [String.prototype.normalize()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/normalize), or
- when attempting to create an array of an illegal length with the [Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array) constructor, or
- when passing bad values to the numeric methods [Number.prototype.toExponential()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number/toExponential), [Number.prototype.toFixed()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number/toFixed) or [Number.prototype.toPrecision()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number/toPrecision).

##
# Code Debugging

Programming code might contain syntax errors, or logical errors.

Many of these errors are difficult to diagnose.

Often, when programming code contains errors, nothing will happen. There are no error messages, and you will get no indications where to search for errors.

Searching for (and fixing) errors in programming code is called code debugging.

##
# The console.log() Method

If your browser supports debugging, you can use console.log() to display JavaScript values in the debugger window:

##
# The debugger Keyword

The debugger keyword stops the execution of JavaScript, and calls (if available) the debugging function.

This has the same function as setting a breakpoint in the debugger.

If no debugging is available, the debugger statement has no effect.

With the debugger turned on, this code will stop executing before it executes the third line.

# HANDLING EXCEPTIONS

If you know that you may get an error, you can handle it gracefully using the try, catch, finally statements. Use them to give your users helpful feedback.

![](201/pic/cc.png)

# TRY

First, you specify the code that you think might throw an exception within the try block. If an exception occurs in this section of code, control is automatically passed to the corresponding catch block. The try clause must be used in this type of error handling code, and it should always have either a catch, fi na 1 ly, or both. If you use a continue, break, or return keyword inside a try, it will go to the f i na 11 y option.

**CATCH**

If the try code block throws an exception, catch steps in with an alternative set of code. It has one parameter: the error object. Although it is optional, you are not handling the error if you do not catch an error. The ability to catch an error can be very helpful if there is an issue on a live website. It lets you tell users that something has gone wrong (rather than not informing them why the site stopped working).

**FI NALLY**

The contents of the fi na 11 y code block will run either way - whether the try block succeeded or failed. It even runs if a return keyword is used in the try or catch block. It is sometimes used to clean up after the previous two clauses. These methods are similar to the .done(), . fail(), and . a 1 ways() methods in jQuery. You can nest checks inside each other (place another t ry inside a catch), but be aware that it can affect performance of a script.