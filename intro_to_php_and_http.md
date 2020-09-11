# Intro to HTTP and PHP

In last year's web programming module. We looked at:-
* HTML
* CSS
* JavaScript

To run our code we simply dragged our HTML pages onto a web browser and the web browser executed the code.

We call these languages **front-end** or **client-side** languages. This is because they are languages that run in a web browser.

This module is primarily about **server-side** or **back-end** web programming and the language we will use is PHP (*PHP: Hypertext Preprocessor*).

A key thing about PHP is that it executes on a web server. Web browsers don't understand PHP. Here's how it works.

1. The client (e.g. a user on their smartphone) using a web browser (e.g. Chrome) and clicks on a link.
2. The web browser sends a **request** out over the Internet to a web server for this resource (e.g. a PHP page). This request uses something called HTTP (Hypertext Transfer Protocol). Here's an example HTTP request that a browser might make.
```
GET /CIT2202/wk01/test.php HTTP/1.1
Host: localhost
User-Agent: Mozilla/5.0 (Windows NT 6.1; WOW64)
```
Requests typically feature more info that this but there are three things we are interested in:
  * The method of the request. This uses **GET**. This is the default method and is used when we want to retrieve data.
  * The server (host) we want to request the PHP page from. In this example *localhost*.
  * The resource we want to retrieve. In this example a file called */CIT2202/wk01/test.php*.
3. The server receives the request and finds the requested resource.
4. PHP code in *test.php* is executed on the web server and plain HTML is sent back to the web browser.
5. The web browser understands HTML and displays the requested page.

> **The key point is that PHP code executes on a web server not in a web browser!**

Now let's have a look at a simple PHP page.

```php
<!DOCTYPE HTML>
<html>
<head>
<title>Simple PHP example</title>
<meta http-equiv="content-type" content="text/html;charset=utf-8" />
</head>
<body>

<?php
echo "<p>Welcome to PHP</p>";
?>

</body>
</html>
```
* To start with we will write PHP by embedding it in an HTML page. So most of this should look fairly familiar to you.
* The page is saved with a *.php* extension e.g. *test.php*
* The PHP tags (```<?php``` and ```?>```) indicate that the enclosed statements are PHP and not HTML. There is only one statement here ```echo "<p>Welcome to PHP</p>";```. *echo* is a command that is used to print output.
* All PHP statements must end with a semi-colon ( ; )

If we request this page from a web server, the following HTML will be retrieved. Have a good look at the two pieces of example code.

```html
<!DOCTYPE HTML>
<html>
<head>
<title>Simple PHP example</title>
<meta http-equiv="content-type" content="text/html;charset=utf-8" />
</head>
<body>

<p>Welcome to PHP</p>

</body>
</html>
```
The PHP code has been executed on the server and plain HTML has been sent to the browser.

PHP isn't the only language used for server-side scripting languages. Here are some others you might come across:-
* Ruby
* Python
* Java
* ASP.NET
