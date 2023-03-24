# 01_BASIC_MODULES

1. Comments in JS are as:-

    ```js
    // THIS IS AN INLINE COMMENT
    /* THIS IS A MULTI-LINE COMMENT */

    ```

2. There are 8 data types which are as:-
    - > undefined, null, boolean, string, symbol, bigint, number, and object

3. Assignment,intializing and assigning to other varaible are as shown:-

    ```js
     var x;
        var a = 0;    // INTIALIZATION OF VARIABLE
        x = 7;        // ASSIGNMENT OF VARIABLE
        a = x;        // ASSIGNING ONE VAR TO OTHER

    ```

4. String Declaration :-

    ```js
    var x = "hello";
    ```

5. Understanding unintialized values:-

    ```js
    var a=5;
    var b=10;
    var c="I am a";
    // Only change code above this line
        
    

    a = a + 1;
    b = b + 5;
    c = c + " String!";
    
    ```
    
6. Diff between var and let and use of const

7. Use of operators and also the compound operators with augmented equations

8. Escaping literal quotes in strings:-

    ```js
    const sampleStr = "Alan said, \"Peter is learning JavaScript\".";
    OUTCOME - Alan said, "Peter is learning JavaScript".
    
    ```
    
9. Concatenating strings:-

    ```js
    const ourStr = "I come first. " + "I come second.";

    ```

10. Escaping Seq:
    - > Code	Output
        \'	single quote
        \"	double quote
        \\	backslash
        \n	newline
        \t	tab
        \r	carriage return
        \b	word boundary
        \f  form feed

11. Construction strings with var:

    ```js
    const myName = "MEET";
    const myStr = "HELLO,MY NAME IS " + myName + ", Good Morning";

    ```

12. Finding length of string:

    ```js
    console.log("Alan Peter".length);

    ```
    
13. Finding char in strings:

    ```js
    const firstName = "Charles";
    const firstLetter = firstName[0]; // firstLetter will have C as value

    ```

14. Assigning string new values:

    ```js
    let myStr = "Jello World";
    myStr = "Hello World";

    ```

15. Word blanks:

    ```js
    It was really ____, and we ____ ourselves ____. 
    const sentence = "It was really " + "hot" + ", and we " + "laughed" + " ourselves " + "silly" + ".";

    ```

16. Storing values in array:

    ```js
    const myArray = ["johny",32];

    ```

17. Nesting of arrays:

    ```js
    const teams = [["Bulls", 23], ["White Sox", 45]];

    ```

18. Accessing array elements:

    ```js
    const array = [50, 60, 70];
    console.log(array[0]); // Prints 50
    const data = array[1]; // Will have 60 as value

    ```

19. Accessing multi-dimension array values:

    ```js
    const arr = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9],
    [[10, 11, 12], 13, 14]
    ];

    const subarray = arr[3];             // will have [[10, 11, 12], 13, 14]
    const nestedSubarray = arr[3][0];    // will have [10, 11, 12]
    const element = arr[3][0][1];        // will have 11

    ```

20. Manipulating arrays with push,pop,shift,unshift:-

    - > /* push() function (adds element at last)

        ```js
        const myArray = [["John", 23], ["cat", 2]];
        myArray.push(["dog",3]) // myArray will have value [["John", 23], ["cat", 2], ["dog",3]]; */

        ```

        /* pull() function (used to remove last element)

        ```js
        const threeArr = [1, 4, 6];
        const oneDown = threeArr.pop();
        console.log(oneDown);               // will have 6
        console.log(threeArr);              // will have 1,4 as values */

        ```

        /* shift() functon (Used to remove first element)

        ```js
        const ourArray = ["Stimpson", "J", ["cat"]];
        const removedFromOurArray = ourArray.shift(); // will have "Stimpson" */

        ```

        /* unshift() function (adds element in beginning)

        ```js
        const ourArray = ["Stimpson", "J", "cat"];
        ourArray.unshift("Happy"); // will contain ["Happy","Stimpson", "J", "cat"] */

        ```

21. Functions :-

    ```js
    function functionName() {
    console.log("Hello World");
    }

    ```

22. Global Scope and Functions :-

    ```js
    // Declare the myGlobal variable below this line
    let myGlobal=10;

    function fun1() {
    // Assign 5 to oopsGlobal here
    oopsGlobal=5;
    }

    // Only change code above this line

    function fun2() {
    let output = "";
    if (typeof myGlobal != "undefined") {
        output += "myGlobal: " + myGlobal;
    }
    if (typeof oopsGlobal != "undefined") {
        output += " oopsGlobal: " + oopsGlobal;
    }
    console.log(output);
    }

    ```

23. Local scope and func

    ```js
    function myLocalScope() {
     // Only change code below this line
    let myVar;
    console.log('inside myLocalScope', myVar);
    }
    myLocalScope();

    // Run and check the console
    // myVar is not defined outside of myLocalScope
    console.log('outside myLocalScope', myVar);

    ```

24. Global vs Local scope in func:-

    ```js
    // Setup
    const outerWear = "T-Shirt";

    function myOutfit() {
    // Only change code below this line
    const outerWear="sweater"
    // Only change code above this line
    return outerWear;
    }

    myOutfit();

    ```

25. Undefined Value returned from a Function:-

    ```js
    // Setup
    let sum = 0;

    function addThree() {
    sum = sum + 3;
    }

    // Only change code below this line
    function addFive() {
    sum=sum+5;
    }

    // Only change code above this line

    addThree();
    addFive();

    ```

26. Assignment with a returned value:-

    ```js
    var processed = 0;

    function processArg(num) {
    return (num + 3) / 5;
    }

    processed = processArg(7);

    ```

27. Boolean values:-

    - >Booleans may only be one of two values: true or false.
    - > Boolean values are never written with quotes. The strings "true" and "false" are not Boolean and have no special meaning in JavaScript.

    ```js
    function welcomeToBooleans() {
   

    return true;

    
    }

    ```

28. Conditional if statement:-
    - >IF CONDITION is true is true,evalutes inside statement or outside braces statement.

    ```js
    function trueOrFalse(wasThatTrue) {
    // Only change code below this line
    if (wasThatTrue) {
        return "Yes, that was true";
    }
    return "No, that was false";
    }

    ```

29. Equality operator:

    ```js
    // Setup
    function testEqual(val) {
    if (val==12) { // Change this line
        return "Equal";
    }
    return "Not Equal";
    }

    testEqual(10);

    ```

30. Strict equality operator:

    ```js
    // Setup
    function testStrict(val) {
    if (val===7) { // Change this line
        return "Equal";
    }
    return "Not Equal";
    }

    testStrict(10);

    ```

31. Comp equality:-

    ```js
    // Setup
    function compareEquality(a, b) {
    if (10 === "10") { // Change this line
        return "Equal";
    }
    return "Not Equal";
    }

    compareEquality(10, "10");

    ```

32. Inequality operator:-

    ```js
    // Setup
    function compareEquality(a, b) {
    if (10 === "10") { // Change this line
        return "Equal";
    }
    return "Not Equal";
    }

    compareEquality(10, "10");

    ```

33. Comparison with inequality operator:-

    ```js
    // Setup
    function testNotEqual(val) {
    if (val != 99) { // Change this line
        return "Not Equal";
    }
    return "Equal";
    }

    // Change this value to test
    testNotEqual(10);

    ```

34. Comp with strict inequality:-

    ```js
    // Setup
    function testStrictNotEqual(val) {
    if (val!==17) { // Change this line
        return "Not Equal";
    }
    return "Equal";
    }

    testStrictNotEqual(10);

    ```

36. Comp with greater than operator:-

    ```js
    // Setup
    function testStrictNotEqual(val) {
    if (val!==17) { // Change this line
        return "Not Equal";
    }
    return "Equal";
    }

    testStrictNotEqual(10);

    ```

37. Comp with >=:-

    ```js
    function testGreaterOrEqual(val) {
    if (val>=20) {  // Change this line
        return "20 or Over";
    }

    if (val>=10) {  // Change this line
        return "10 or Over";
    }

    return "Less than 10";
    }

    testGreaterOrEqual(10);

    ```
38. Comp with less than operator:-

    ```js
    function testLessThan(val) {
    if (val<25) {  // Change this line
        return "Under 25";
    }

    if (val<55) {  // Change this line
        return "Under 55";
    }

    return "55 or Over";
    }

    testLessThan(10);

    ```

39. Comp with <= :-

    ```js
    function testLessOrEqual(val) {
    if (val<=12) {  // Change this line
    return "Smaller Than or Equal to 12";
    }

    if (val<=24) {  // Change this line
        return "Smaller Than or Equal to 24";
    }

    return "More Than 24";
    }

    testLessOrEqual(10);

    ```

40. Comp with logical operator:-

    ```js
    function testLogicalAnd(val) {
    // Only change code below this line

    if (val>=25 && val<=50) {
        
        return "Yes";
    
    }

    // Only change code above this line
    return "No";
    }

    testLogicalAnd(10);

    ```

41. Logical Or operator:-

    ```js
    function testLogicalOr(val) {
    // Only change code below this line

    if (val < 10 || val > 20) {
        return "Outside";
    }

    // Only change code above this line
    return "Inside";
    }

    // Change this value to test
    testLogicalOr(15);

    ```

42. Else statements:-

    ```js
    function testElse(val) {
    let result = "";
    // Only change code below this line

    if (val > 5) {
        result = "Bigger than 5";
    }
    else {
    return "5 or Smaller";
    }

    

    // Only change code above this line
    return result;
    }

    testElse(4);

    ```







    

