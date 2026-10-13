# API Testing
* Presentation Layer (GUI)
* Application Layer
* Data Layer
* FOUR TYPES OF API:
 - Open APIs (Public APIs)
 - Internal APIs (Private APIs)
 - Partner APIs
 - Composite APIs (These combine multiple APIs into one call, allowing you to get data from different sources in a single request)
* If you place API in the production, you call it as a web service. **_** All web services are APIs but every APIs is not web service.**_**
* Whatever APIs are available in the internet, we call them as a web service.
* MICROSERVICE is a small functionality in the application.
* Microservices communicate each other via APIs.
* We have REST and SOAP APIs. SOAP APIs are older and very less companies are using.
* SOAP APIs are using only Xml format sending request and response.
* REST APIs--> JSON, XML, text format, HTML, CSV format.
* REST APIs are faster than SOAP APIs.
* Difference between HTTP and HTTPS: HTTP is not secured, actually your data is not secured. HTTPS-->your data is secured, encrypted.
* URI--> Uniform Resource Identifier
* URL--> Uniform Resource Locator
* URN-->Uniform Resource Name
* FEATURE: is the term used in manual testing to test some functionality.
* RESOURCE: is the term used in API Automation testing referring some functionality.
* PAYLOAD--> means **body** in the HTTP request and response message.
* C - Create -->POST
* R - Retrieve -->GET
* U - Update -->PUT
* D - Delete -->DELETE
* A collection is a group of requests.
* https://reqres.in/api/users?page=2
* HOW TO CREATE APIs:
 - NodeJS
 - NPM (comes with NodeJS)
 - JSON-server (C:\Users\niyaz>npm install -g json-server)
 * to create your own API: C:\Users\niyaz\Downloads\back_end testing>json-server --watch student.json)


# JSON (JavaScript Object Notation):
* JSON is a syntax for storing and exchanging data.
* Basically, it was designed for human-readable data interchange.
* JSON is text, written with JavaScript Object Notation.
* It has been extended from the JavaScript scripting language.
* The filename extension is .json.
* JSON Internet media type is application/json.
  


# JSON Data Types
1. String: A string in JSON is a sequence of characters enclosed in double quotes (""). It can include letters, numbers, spaces, and special characters.
2. Number: in JSON can be integers or floating-point (decimal) values. They do not require quotes.
3. Boolean: Boolean values can either be true or false. They represent binary states and are not enclosed in quotes (e.g. {"isStudent:true, "isEmployed": false}).
4. Null (e.g. {"middleName":null})
5. Array: An array is an ordered list of values. The values can be of any JSON data type (e.g., strings, numbers, objects, etc.). Arrays are enclosed in square brackets (`[]`).

**Example:**

```json
{
  "skills": ["Java", "Python", "Selenium"],
  "scores": [85, 90, 95]
}
```
6. Object :An object is a collection of key-value pairs enclosed in curly braces (`{}`). Keys are strings, and values can be any JSON data type.

**Example:**

```json
{
  "person": {
    "firstName": "John",
    "lastName": "Doe",
    "address": {
      "city": "New York",
      "zip": "10001"
    }
  }
}
```

* 7. Example Combining All Data Types**

Here is a more complex example that combines all JSON data types:

**Example:**

```json
{
  "name": "Alice",
  "age": 28,
  "isMarried": false,
  "children": null,
  "hobbies": ["reading", "traveling", "coding"],
  "address": {
    "city": "Los Angeles",
    "state": "California",
    "postalCode": "90001"
  },
  "scores": [95.5, 88.0, 76],
  "profileComplete": true
}
```

# JSON Example:
{
"Title": "The Cuckoo’s Calling",
"Author": "Robert Galbraith",
"Genre": "classic crime novel",
"Detail": {
   "Publisher": "Little Brown",
    "Publication_Year": 2013,
    "ISBN-13": 9781408704004,
    "Language": "English",
    "Pages": 494
       },
"Price": [
{
"type": "Hardcover",
"price": 16.65
},
{
"type": "Kindle Edition",
"price": 7.03
}
]
}

# JSON Path

* JSON Path is a query language for JSON data, similar to XPath for XML. 
* It allows you to navigate and extract specific data from a JSON document by specifying paths. 
* JSON Path uses a syntax that makes it easy to access elements, objects, arrays, and their nested components.

# JSON Path Syntax Overview

1. Dot Notation (.): Accesses child elements.
2. Bracket Notation ([]): Accesses array elements or specific keys.
3. Wildcard (*): Matches all elements.


{
 "store": {
   "book": [
     {
         "title": "Java Programming",
         "author": "John Doe",
         "price": 29.99,
         "categories": ["Programming", "Java"]
     },
     {
        "title": "Python Basics",
        "author": "Jane Smith",
        "price": 19.99,
        "categories": ["Programming", "Python"]
    }
],
"bicycle": {
    "type": "Mountain",
    "price": 499.99
  }
 }
}

* I want to access Mountain ---> $.store.bicycle.type
* I want to access Python Basics--> $.store.book[1].title


# Useful tools to generate and evaluate JSON Paths:

* https://jsonpathfinder.com/](https://jsonpathfinder.com/
* https://www.site24x7.com/tools/jsonpath-finder-validator.html
* https://jsonpath.com/


# 4. VALIDATING RESPONSE inPOSTMAN & JS
* 