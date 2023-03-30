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

43. Introducing else if statements:-

    ```js
    function testElseIf(val) {
    if (val > 10) {
        return "Greater than 10";
    } else if(val < 5) {
        return "Smaller than 5";
    } else {
        return "Between 5 and 10";
    }

    }

    // Change this value to test
    testElseIf(7);

    ```

44. Logical order in else if statements:

    - > Order is important in if, else if statements.
    - > The function is executed from top to bottom so you will want to be careful of what statement comes first.

    ```js
    function orderMyLogic(val) {
    if (val < 5) {
        return "Less than 5";
    } else if (val < 10) {
        return "Less than 10";
    } else {
        return "Greater than or equal to 10";
    }
    }

    orderMyLogic(7);

    ```

45. Chaining of if/else:-

    ```js
    function testSize(num) {
     // Only change code below this line
    if(num<5){return "Tiny";}
    else if (num<10) {
    return "Small";
    } else if (num<15) {
    
    return "Medium";
    } else if(num<20){
    return "Large";
    }
    else if(num>=20){
    return "Huge";
    }
    else{return "Change Me";}
    // Only change code above this line
    }

    testSize(7);

    ```

46. GOLF CODE :-

    - >In the game of Golf, each hole has a par, meaning, the average number of strokes a golfer is expected to make in order to sink the     ball in the hole to complete the play

    ```js
    const names = ["Hole-in-one!", "Eagle", "Birdie", "Par", "Bogey", "Double Bogey", "Go Home!"];

    function golfScore(par, strokes) {
    // Only change code below this line
    if (strokes == 1) {
        return names[0];
    } else if (strokes <= par - 2) {
        return names[1];
    } else if (strokes === par - 1) {
        return names[2];
    } else if (strokes === par) {
        return names[3];
    } else if (strokes === par + 1) {
        return names[4];
    } else if (strokes === par + 2) {
        return names[5];
    } else {
        return names[6];
    }
    // Only change code above this line
    }

    // Change these values to test
    golfScore(5, 4);

    ```

47. Selection from switch statements:-

    - >If you have many options to choose from, use a switch statement. A switch statement tests a value and can have many case statements    which define various possible values. Statements are executed from the first matched case value until a break is encountered.

    ```js
    function caseInSwitch(val) {
    let answer = "";
    // Only change code below this line
    switch (val) {
        case 1:
        answer = "alpha";
        break;
        case 2:
        answer = "beta";
        break;
        case 3:
        answer = "gamma";
        break;
        case 4:
        answer = "delta";
        break;
    }
    // Only change code above this line
    return answer;
    }
    // Change this value to test
    caseInSwitch(1);

    ```

48. Switch statements types of modules:

    - > Learned to add default statement 

    - > Learned multiple identications

    - > Replaced if/else statements with switch

49. Replacing Boolean values from functions:-

    ```js
    function isLess(a, b) {
    // Only change code below this line
    return a<b;
    // Only change code above this line
    }

    isLess(10, 15);

    ```

50. Return Early Pattern for Functions

    - > When a return statement is reached, the execution of the current function stops and control returns to the calling location.

    ```js
    // Setup
    function abTest(a, b) {
    // Only change code below this line
    if (a < 0 || b < 0) {
        return undefined;
    }


    // Only change code above this line

    return Math.round(Math.pow(Math.sqrt(a) + Math.sqrt(b), 2));
    }

    abTest(2,2);

    ```

51. Javascript Objects:-

    - > Objects are similar to arrays, except that instead of using indexes to access and modify their data, you access the data in objects through what are called properties.

    ```js
    const myDog = {
    // Only change code below this line
    "name":"Beuno",
    "legs":4,
    "tails":1,
    "friends":["cats","pets"]

    // Only change code above this line
    };

    ```

52. Accessing Object Properties with Dot Notation:-

    - > There are two ways to access the properties of an object: dot notation (.) and bracket notation ([]), similar to an array.

    ```js
    // Setup
    const testObj = {
    "hat": "ballcap",
    "shirt": "jersey",
    "shoes": "cleats"
    };


    // Only change code below this line
    const hatValue = testObj.hat;      // Change this line
    const shirtValue = testObj.shirt;    // Change this line
    
    ```

53. Accessing Object Properties with Bracket Notation

    ```js
    // Setup
    const testObj = {
    "an entree": "hamburger",
    "my side": "veggies",
    "the drink": "water"
    };

    // Only change code below this line
    const entreeValue = testObj["an entree"]   // Change this line
    const drinkValue = testObj["the drink"];    // Change this line

    ```

54. Accessing Object Properties with Variables

    ```js
    // Setup
    const testObj = {
    12: "Namath",
    16: "Montana",
    19: "Unitas"
    };

    // Only change code below this line
    const playerNumber = 16;  // Change this line
    const player = testObj[playerNumber];   // Change this line

    ```

55. Add New Properties to a JavaScript Object

    ```js
    const myDog = {
    "name": "Happy Coder",
    "legs": 4,
    "tails": 1,
    "friends": ["freeCodeCamp Campers"]
    };

    myDog.bark="woof";

    ```
    
56. Dlt prop of js obj:-

    ```js
    // Setup
    const myDog = {
    "name": "Happy Coder",
    "legs": 4,
    "tails": 1,
    "friends": ["freeCodeCamp Campers"],
    "bark": "woof"
    };

    // Only change code below this line
    delete myDog.tails;

    ```

57. Using obj for lookups:-

    ```js
    // Setup
    function phoneticLookup(val) {
    var result = "";

    var lookup = {
        "alpha": "Adams",
        "bravo": "Boston",
        "charlie": "Chicago",
        "delta": "Denver",
        "echo": "Easy",
        "foxtrot": "Frank"
    };
    // Only change code below this line

    result = lookup[val];

    // Only change code above this line
    return result;
    }

    // Change this value to test
    phoneticLookup("charlie");

    ```

58. Testing obj for prop:-

    ```js
    // Setup
    function checkObj(obj, checkProp) {
    if (obj.hasOwnProperty(checkProp)) {
    return obj[checkProp];
    } else {
    return "Not Found";
    }
    }

    ```

59. Manipulating Complex Data:-

    ```js
    const myMusic = [
    {
    "artist": "Billy Joel",
    "title": "Piano Man",
    "release_year": 1973,
    "formats": [ 
    "CS", 
    "8T", 
    "LP" ],
    "gold": true
    },
    // Add record here
    {
    "artist": "Bob",
    "title": "Hello",
    "release_year": 1950,
    "formats": [
    "CS",
    "8T"
    ]
    }

    ];

    ```

60. Accessing nested obj:-

    ```js
    // Setup
    var myStorage = {
    "car": {
    "inside": {
    "glove box": "maps",
    "passenger seat": "crumbs"
    },
    "outside": {
    "trunk": "jack"
    }
    }
    };

    // Only change code below this line

    var gloveBoxContents = myStorage.car.inside["glove box"]; // Change this line

    ```

61. Accessing Nested Arrays:-

    ```js
    // Setup
    var myPlants = [
    {
        type: "flowers",
        list: [
        "rose",
        "tulip",
        "dandelion"
        ]
    },
    {
        type: "trees",
        list: [
        "fir",
        "pine",
        "birch"
        ]
    }
    ];

    // Only change code below this line

    var secondTree = myPlants[1].list[1]; // Change this line

    ```
    
        





        

