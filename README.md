## Chai aur Javascript ☕

### Lecture 1:

- Getting confidence in software development is very important
- Doing porject will gives you the confidence
- confidence will only clear the interviews
- No extra tool required to setup to learn javascript
- Now will cover the latest javascript

### Lecture 2: Setting up local environment

- Javascript execution is same for browser or running on any environment
- Every source code has meaning in javascript, like console.log() has some meaning in javascript, it is syntax in programming language
- Every programming language comes with some extenstion like .js, .py
- Every software has capability to understand the syntax whether it is .js or .py, which we call interpretor or compiler
- The compiler / interpretor was hidden in browser but now taken out in nodejs enviroment
- Now we no need to write, index.html and create the seaprate js file and add in script, as it was attached with broweser.
- Now we can run javascript directly with node environment, Hence Javascript is used everywhere like in frontend, backend etc
- Install the nodejs from nodejs.org and run in the local machine
- For writing the code use, VS Code, as it very popular now a days, it is from microsoft
- VS Code will help in color correction, indentation etc
- Go to view --> terminal, here you can see the terminal
- check whether node is installed or not: node -v, our work done, if we get some number like 18, then we are ok
- To execute the code, we use: node filename

### Lecture 3: Github

- We have lot of online code execution environment available like Github
- Lets see, how can we setup the code environment in github

  - Go to github and create the account
  - Create new repository --> code-with-javascript-one
  - Create the README.md and create the repository
  - There are different to use github, but here we will see codespace
  - click on code --> codespaces
  - We will get the vscode here, here wee will get the computer like environment
  - Here click file --> view --> command palletter --> write 'Container' --> Add Dev container Configuration Files
  - it means, we are adding the configuration files
  - click Show all configuration --> node.js & Javascript --> click default --> ok --> rebuild --> it will add some execution files
  - How to push the code to the githib:
    - 1. click on source control --> add the file on + click --> add message --> click on commit
    - 2. click on triple dot --> click on push
    - reload the github to get the files updated
  - To stop the github codespaces
    - click on codespace --> see owned by 'username' on right side --> click on 3 dot --> delete the working directory --> ok
    - We can start the machine when needed

### Lecture 4: Variables & Constants

    - Only people will survive in the Tech indutry whos motive is to create something product
    - Through javascript, we can create, mobile app, web app etc
    - Set goal to create Ecommerce app or social media app
    - All game is about mindset, here mideset to create a sample product
    - Think to create a ecomerce app
        - I need to attract user and make him into register
        - given him/her unique id
        - When user comes --> he enter the details like name, city, etc, it needs to store --> it ll stored in memory space, here it is varaible later DB ha
        - Here, all the game is about, storing the data and retriving it
        - so we learn variable and constants
    - variable can be change but constant is constant
    - we will learn about investigation
    - we should the name that is easily readable
    - When we see the var, let, const, it means, we need to assign in memory
    - const means, we cant change the value, it will through an error, if we try to change the constant value
    - to write a comment, we use // 2 slashes, it means, javascript cant execute this lines
    - we can print multiple values in console.log([]) like this by separting commas
    - in js, let and const and be done using let and const
    - in js, there was a problem of scope, means anything written in {}
    - in js, when some programmer change the value in scope, it will impact the existing varaible
    - so in modern js, we use let, const to overcome the issue of block scope and function scope
    - /* */ this is also way of comment
    - we caen reserve the variable without using anykeyword as well, but it is not good practice
    - In js, semicolon is optional
    - Defualt value of let is undefined

    ## Lecture 5: Datatypes

    - Prefer to practice on keyboard rather then taking notes on paper, write notes here itself so to remember
    - "use strict" if we use above 2 words, it means it is newer version of javascript
    - alert("hello") if we run the code, it ll given an error saying node is not defined, as js engine is hidden in browser --> it means, to run alert() has different way ti run it.
    - In coding readability is very important ans it should be future proof
    - for documentation prfer mdn (mozilla documentation)
    - Original documenataion would be find in tc39.es
    - ECMA Script is the standard way of writing javscript
        -    for example,  if we write loop, then we should write in this way etc
    - In js , we have different datatype,
        - Primitive Datatype:
            - like number, string, boolean, null, undefined, bigInt, symbol
    - Prefer to use double quotes for string datatype
    - Boolean will say yes or no, it has only 2 values
    - null --> it is standalone value, yes it is datatype as well
        - null is representaiton of empty value
        - null means value is empty, example, like giving empty value while monitoring the temp, as we cant give 0, as 0 has some value in temp scale
    - undefined --> means some value is not defined
    - Symbol datatype is used to fincdout the uniquness --> it is used in react, to find the component
    - typeof --> to know the type of any variable, we use typeof
        - example: console.log(typeof "sarfaraz") --> string
    - commit and push the change

    ## Lecture 6: Conversion Operation

    - we dont in javascript, what type of value we get, so we need to use conversion of datatype
    - we can write typeof in 2 ways
        - typeof variablename
        - typeof(variableName)
    - To convert string into Number, we use Number(variableName);
    - When value is not proper number like 33abc, its type is NaN
    - In Javascript, there is no strict check, so we use typescript
    - conversion of null into number is 0
    - conversion of undefined into number is NaN
    - Conversion of boolean into number is false
    - Conversion of string into number is NaN, as it is not able to convert into number
    - Number conversion summary:
        - "33" => 33
        - "33abc" => NaN
        - true => 1; false =>0
    - it is very important to know, is the value is converted and know what value it gives us back.
    - conversion of 1 gives true
    - conversion of "" emty string gives false;
    - Boolean conversion summary:
        - 1 => true, 0=> false
        - "" => false
        - "Sarfaraz" => true

### Lecture 7: Operations

    - if string is 1st then all conversion will into string
        - example: console.log("1"+2+2) --> 122
    - if the string is last then conversion will be done before that then string will be added
        - example: console.log(1+2+"2") --> 32
    - should know about more about convertion: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Increment

### Lecture 8: Comparisons

    - comparison shouild be done with same datatype only
    - here console.log("2" >1) will be converted into 2>1 condition, here the auto conversion happens
    - while comparion null is converted into 0 or NaN, example console.log(null > 0), means 0 > 0, hence answer is false. So avoid only value check but use value with datatype check.
    - comparison with undefined with 0 is always false, example: console.log(undefined == 0); it gives false
    - In Javascript, comparison and equality check both work differently
    - ==== Strict check, it will check value as well as data type

### Lecture 9: Datatype summary

    -  Datatype is basically into 2 types
        - primitive
        - Non-primitive
    - Difference between is call by value and call by reference, it means how we are saving the data into memory and how we are accessing the data
    - Primitive Datatype:
        - Primitive is into 7 categories
        - Prmitive datatype is call by value
        - when we take the data, it is copied, so the changes are done on copied data
        - String, Number, Boolean, null (meam empty), undefined, Symbol (to make the value unique), BigInt
    - Non-Primitive Datatype
        - It is also called as reference type
        - we can get the reference of the available data
        - Array, Objects, Functions

    - *** To master the javascript,
        - learn Objects and browser events

    - JavaScript is a dynamically typed language, which means that data types of variables are determined by the value they hold at runtime and can change throughout the program as we assign different values to them
    - For big integer number, we add n at the end of the number.
    - Object is declared with curly brases
    - Datatype of function is called object function
    - Documentation link: https://262.ecma-international.org/5.1/#sec-11.4.3

### Lecture 10: Stack and Heap Memory

    - Memory is of 2 types 1. Stack 2. Heap Memory
    - Stack memory is used for primitiva datatype while heap memory is used for non primitive datatype
    - To draw online diagram use: https://excalidraw.com/
    - we will get original value reference when take back the value from reference value
    - Whatever goes in heap, we only get the reference, means whatever changes we are doing, we are doing in original value
    - From stack, we get the copy of the value

### Lecture 11: String in javascript

    - Through string, we can use modern syntax to write it.
    - We denote string single or double quote '' / ""
    - in modern days, we need to use backticks `` for strin manipulation called string interpolation.
    - All methods are available in __proto__ for string, example toUpperCase() etc
    - If we use methods related to __proto__ then original value is not changed.
    - we can check what character available we use charAt(index)
    - indexOf('charactor') : we can get the index of the charactor
    - in substring(0,4) the last value is excluded.
    - trim() : this method is used to remove the unwanted space, mostly it is used in filling the form
    - split('-') : split mothod is used to split with specified digit and gives the output in arrays

### Lecture 12: Numbers and Maths

    - If we write const score=400, then Javscript will recognise it as number, but we can explicitly define numbers as new Number(400)
    - we can convert number into string using toString() method, it will help me to use string methods
    - toFixed() :  to give the precision value till few decimal values, like toFixed(2) --> it wwill give .00 like that
    - toPrecision(3):  it will focus on only 3 digit value only
    - toLocaleString('en-IN') : this method will be helpful in giving the output in redable format of number, like 1000000 --> 1,000,00
    - Maths.abs(): it will convert -ve value into +ve value, +ve will remain +ve, it helps to convert valeue into +ve value.
    - Math.round(): To get the round value, example: Math.round(4.3) --> 4
    - Math.ceil(): It will round the value to top. Example: Math.ceil(4.6) --> 5 or Math.ceil(4.2) --> 5
    - Math.floor(): It will take bottom value, Example: Math.floor(4.2) -6-> 4.2 or Math.floor(4.6) --> 4, It will always takes the lowest value
    - Mostly we will use round() method instead of ceil and floor
    - Math.min(): we can findout the minimum value from the given numbers, example: Math.min(3,4,5,6,) --> 3
    - Math.max(): we can findout the maximum value from the given numbers, example: Math.min(3,4,5,6,) --> 6
    - random(): it will the random value between 0 and 1
        - To make the value in 1 digit then add 1, example: (Math.random()*10)+1
        - We can round of the value using Math.floor in random method
        - We can add 10, if we want the value more then 10

### Lecture 13: Date and Time

    - Reference: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date
    - Date is calculted in milli second starting from January 1st
    - In future, we will be using Temporal object like Math, which will contain all the methods, but as of we will be using Date object only.
    - Date can be converted into string using toString() method
    - toLocaleDateString(): It will give the value with date with / format Example: 9/27/2023
    - toLocaleString(): It will give the date value with time with / format Example: 9/27/2023, 7:05:46 PM
    - In short: Every date method will add or remove some format
    - Data type of Date is object
    - Note: Month will start from 0 in javascript, but when we give the date in format it starts with 1, Example new Date("2023-01-23") --> 1/23/2023
    - timestamp will be used, when we want to give the polls, like who has given the fastest answer
    - Date.now(): It will give the current date in milli second
    - We can get the details about date using other method starting with get,
        - Example: let newDate = new Date();  console.log(newDate.getMonth()+1) --> 9, added 1 as date always starts with 0.
    - We can customise the date format, Example: newDate.toLocaleString('default',{ weekday: "short"}) --> Wed, as today is Wednesday

### Lecture 14: Array

    - Array has squre brakcet, Array has elements in it.
    - Documentation: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array
    - We can store the muliple values in single variable
    - Javascript array are resizable
    - Array indexing starts with 0
    - we can access the array using indexing, Example: myArr[0]
    - When we copy array, the array creats shallow copy, means share same reference point, means, it will change the original array, while Deep copy do not share the same reference
    - We can declare the array using 2 types
        - using square brakcet []
        - using new Array(). here it will add the square bracket by its own
    - We can view all the methods available in array.
        - Example: const numbers = [1,2,3,4]; console.log(numbers) --> click on prototype to see the methods
    - Array contain the mixed data type
    - Array ha prototype proerty access
    - Array has length property , to calculate the length of an array
    - push(): It will add the value in the array
    - pop(): Remove the last available value in array
    - unshift(): Value will be added at the start, But here problem is, we need to shift all values to right
    - shift(): remove the first element from an array
    - Some array method will answer in yes or no, like includes(), so based on true or false, we can write the condition and judge the value
    - join(): add all the element in the array but gives output into string
    - slice(): It will not update the orignal array, here last range is not included, will give the extracted array from start to end value
    - splice(): It will update the original array, Gives the extracted array as output.
    - concat(): It will combine 2 arrays and gives the new array
    - spread operator: think glass of water, when glass fall --> water spread to the ground : remember
        - in spread operator, we will get the spread out values
    - flat(): This method is used to flatten the array, we need to mention the depth as a pramater
    - Array.isArray(): To check the given array is array or not, it will give true or false response
    - Array.from(): this method will convert any given number/name into array
        - If we pass an array in from, then we need to mention, do we need to create the array for keys or values
    - Array.of() : Will give the newly formed array, will convert any values into new array

### Lecture 15: Objects

    - To master javascript, we need to learn 2 things
        - Objects
        - Events
    - Objects can be declared in 2 ways
        - Literal
        - Constructor
    - Singleton: It means, only 1 object is created.
        - When the object is created using constructor, it is singleton
        - Example: const JsUser = {}
    - Object has keys and values
    - By Default key is in the string format in object
        - To access the object element, we use JsUser["name"] , it means we are accessing using string
    - we can update the value of the user using = equal to
    - We can freeze the object using Object.freeze() to avoid the further update
    - To define Symbol, we use square bracket [], it says I am a symbol
    - function can be treated as a varaible in javascript
    - we can get the reference if we dont give paranthesis in function call with object, example: JsUser.greeting --> [Function (anonymous)]
    - if we want to reference the same object, then we can use 'this'

### Lecture 16: Objects 2: Object using constructor

    - We can create the object using {} or new Object(), here both are same
    - We can have any level of nesting in object
    - we can access the object key using [], for nested value we can use [][], Example : regularUser["fullname"]["userfullname"]["firstname"]
    - We can use optional chainging to avoid the error: ?.
    - Object.assign(): This method copies all the values of an objects
    - We can extract keys using Object.keys and values using Object.values from an object
    - Object.entries() : To get all the values of object in key value pair
    - hasOwnProperty(): To check the property exists in object or not
    - To check the different mehoda available in object, use this trick
        - go to browser console
        - const obj1 = {1:"a",2:"b"} --> obj1 --> chec all the methods in [prototype]

### Lecture 17: Objects Destrcuturing and JSON API

    - object destructuring is a syntactically sugar, means it only provide the syntax
    - object destructuring helps in avaoiding the repeatability of the code
    - In Object destructuring, we are extracting the property from object
    - We can rename the destructure value using colon :
    - When we go to the restaurant and order something, the menu card is API Documentation
        - When we order 'Samosa', we should not worry how it is made, just we have cOnsume it, Somosa is created at the backend, same goes with API.
    - JSON is almost written like object, but key, value pair are stored in string
        ```json
        {
            "name": "hitesh",
            "coursename" : "js in hindi"
        }
        ```
    - Use the url : https://api.github.com/users/hiteshchoudhary
    - Use the API --> As the value is into JSON --> convert in javascript object --> use it, enjoy
    - Famous API: Random user me: https://randomuser.me/ --> use https://randomuser.me/api/
    - We can beautify the JSON using JSON Formatter online editor: https://jsonformatter.org/ --> we can beautify the JSON and check it into tree structure --> after this we can see how can we deal with it, may be using array or object

### Lecture 18: Functions and parameters

    - While learning about functions, it is important to know about memory management as well.
    - Function means, what the 10, 20 etc lines of code you have writte, we kept in package
        - We can resue the package, as much as we want
        - To write a function, we give function keywoes, function name, then pranthesis then scope of function, this is called function defination
        - To call the function, we function name with parenthesis, then function will execute it.
    - In javascript, it automatically check the datatype of value, so it is important to check the type of any variable before doing any operations
    - function parameter : while creating the function defination, whatever the inputs we take, we call it as parameters
    - function arguments: The values which we pass in the function call, we call it as an argument
    - It is important to know, what we are sending form the function
    - **Note: Whatever you write after function return, nothing will work
    - undefined and "" empty string is considered as false value
        - So to check the error, check with false value --> Example:  if(!username)
    - We can give default value in function parameter with equals to, Example loginUserMessage(username = "sam")  --> it will avoid to go into error check, if no username available
    - Rest Operator: ... when these 3 dots comes in parameter, it means get all the values and give me in bundle.
        - Example: Get all the values in cart value

### Lecture 19: Global and local scope

    - Scopes story starts with var, let and const
    - {} :  This is called as scope
    - when {} comes with function or if, then we called its scope
    - When any thing declared inside {} it is called block scope, and outside of {} is called global scope
    - value declare in global scope --> it is available in block scope but value declaredin block scope is not available in global scope.
    - var is functional scope, where as const, let are block scope.
    - Global scope is different for node environment and browser

### Lecture 20: Scope level and mini hoisting

    - {} Is only scope in javascript ha
    - Kids can ask ice cream from elder but it is awekword if elder ask the ice cream from kids
        - It means, inner function can access the variable from outside but outside function cant ask inner member variables etc
    - Variable declared inside the insode function cant be access outside function
    - Every time function is called, then every time it is kept in stack
    - Closure in simple line, the inner function can access the outside declared variable
    - There are 2 technique to create a function, using bassic function, other is function expression
    - Hositing is not possible with function expression, but hoisting is possible with basic function only

### Lecture 21: this and arrow function

    - ES6 came in 2015 and came with lots of new features
    - arrow function and this keyword are the features of ES6
    - this keyword tells about current context
    - when we refer to the current context of the object, we use this keyword
    - In node environment, current object refer to empty object
    - node javascript engine is stand alone, earlier javascript engine is in a browser
    - In brower there is a global object called window object
    - this keyword is not accessible in noraml function and function expression (doubt)
    - To write arrow function, replace function keyword with qual and arrow in function expression
    - note: this keyword can be accessible in normal function, act as a global object but not in arrow function
    - syntax of arrow function: const sampleArrowFunction = ()=> {}
    - ** Implicit Return: when arrow function is 1 liner, then we consider it as implicit return and no need to write the return keyword
    - if use curly braces, --> then need to use return. If we use paranthesis, then no need to add the return keyword.
    - To return the object, we should wrap in parenthesis

### Lecture 22: Immedietly Invoked function

    - The function which has its own scope and executed immideitly
    - IIFE: Function defination is wrapped in paranthesis and use empty parenthesis for execution: ()()
        - Note: To avoid the use of global variable, as global variable pollute the variable, so we use IIFE
        - Note: To stop the IIFE, It is important to add the semicolon after IIFE
        - We can write IIFE using normal function as well as arrow function
        - Remember 2 IIFE can be written by seperating semicolon

    ## Lecture 23: Javascript Behind scene

    - Remember how the call stack works in javascript
    - Javascript Execution context:  it means, the javascript created by you, how it will run
    - Javascript has 2 execution context:
        1.  Global execution context: It is store in 'this', executed in thread, remember javascript is single threaded language
        2.  Functional execution context
    - Javascript runs the code into 2 phases
        1.  Memory creation phase:
            - Memory is created for variables and functions declared, it is not executed here
            - just variables are created, and kept with us
        2.  Execution Phase:  we will get all the values
    - lets see with the example:

            - ```javascript
                let val1 = 10;
                let val2 = 5;
                function addNum(num1, num2){
                    let total  = num1  + num2;
                    return total;
                }
                let result1 = addNum(val1, val2)
                let result2 = addNum(10, 2)
                ```
            1.  Memory Creation Phase: Here, In 1st cyle we will get
                - val1 -> undefined
                - val2 -> undefined
                - addNum -> defination
                - result1 -> undefined
                - result2 -> undefined
            2.  Execution Phase:
                - val1  <- 10
                - val1  <- 5
                - For addNum function, now different execution phase will be created
                    - 1. New variable environment
                    - 2. Execution thread
                        - Memory phase:
                            - val1 -> undefined
                            - val2 -> undefined
                            - total -> undefined
                        - Execution context: Here execution happens
                            - num1 -> 10
                            - num2 -> 5
                            - total -> 15 --> total will return to global execution context
                        - The execution context will be deleted after the work is done
                        - result1 -> 15
                        - result2 -> here again 2 phased will be created
                            - 1. Memory phase
                            - 2. Execution Phase
                            - here again the total will be calculated and sent to the execution context
            - Callstack: All the method will be executed here, it will be removed once the work is done
                - It follow the LIFO
                - we can check the flow of function call by giving break points

### Lecture 24: Control flow ☕

    - In if statement, if the condition is true then only code will execude for if statement
    - if statment will be having comparison statement
    - Following are the comparator operators checking:
        - less then < --> Example: 10 < 20 --> check 10 is less then 20, yes it is, so output: true
        - greated then >
        - less then and equal to <=
        - greater then and equal to >=
        - Equal to ==, note single operator is assignmnet operator, Example: const isLoggedIn = true, means true is assigned to isLoggedIn, but here == is comparison operator
        - Not Eqaul != --> 3 !=2 --> -ve checking --> 3 is not equal to 2 --> output: true
        - === will check the type and value, it is strict equality check
        - !== It will do -ve type and value checking
        - else is conditional code, it will executed either if statement or else statement
        - scope is counted in curly braces {}
        - var scope is compltely global, it means, it accessable outside {} as well
        - && : and condition will check both left and right condition
            - Example: Do you need to buy phone and cover --> yes
            - if any of the condition is wrong in &&, the block will not get executed
        - || : called pipe sign, help to multiple check or condition

        #### Switch case:

        - Using switch case, we will be checking multiple values
        - syntax:
            ```javascript
            switch(key){
                case value:
                    break;
                default:
                    break;
            }
            ```
        - here key is the condition, we need to check everytime
        - use intellesence or seuggestion in vscode for switch case
        - if nothing match, then default case will be excuted
        - whenever, key is match rest all code will be executed, so we give break to avoid limited details to show

        #### Truthy & flasy values

        - Any value added in string is truthy value
        - [] empty arry, empty object are truthy value
        - if only function is declared, then that is also truthy value
        - Object.key() will return the array
        - Remember: it is true comparison below
            - false == 0 --> true
            - false == '' --> true
            - 0 == '' --> true
        - && || are called logical operator

        #### Nullish Coalescing Operator (??)

        - Need to focus on Null and undefined values
        - ?? it will check the safty value, based on null or undefined it will assign some other value
        - while using ?? operator twice, it will take the 1st assigned value, Example: null ?? 10 ?? 10 --> output: 10
        - ?? is basically used to handle errors
        - nullish and null operator are 2 different thing
        - Ternary operator: it is short cut of writing if else statement
            - Syntax: condition ? true : false

### Lecture 25: for loop, break and continue

    - use ctrl + d : to select the multiple value at once
    - To stop any control, we use break keyword
    - continue is like, sorry for 1 time (means skip when the condition match) and continue the process remain

### Lecture 26: while, do while loop

    -

### Lecture 27: Higher order array loops

    -

### Lecture 28: filter, map and reduce

    -
