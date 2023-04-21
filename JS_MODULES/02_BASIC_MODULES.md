# ECMA-SCRIPT MODULES

1. Compare Scopes of the var and let Keywords

    ```js
    function checkScope() {
    "use strict";
    let i = "function scope";
    if (!true) {
        i = "block scope";
        console.log("Block scope i is: ", i);
    } else {
    console.log("Function scope i is: ", i);
    return i;
    }
    }

    ```

2. Mutate an array declared with const:-

    ```js
    const s = [5, 7, 2];
    function editInPlace() {
    // Only change code below this line
    s[0]=2;
    s[1]=5;
    s[2]=7;
    // Using s = [2, 5, 7] would be invalid

    // Only change code above this line
    }
    editInPlace();

    ```

3. Prevent obj mutation;

    ```js
    function freezeObj() {
    const MATH_CONSTANTS = {
        PI: 3.14
    };
    // Only change code below this line
    Object.freeze(MATH_CONSTANTS);

    // Only change code above this line
    try {
        MATH_CONSTANTS.PI = 99;
    } catch(ex) {
        console.log(ex);
    }
    return MATH_CONSTANTS.PI;
    }
    const PI = freezeObj();

    ```

4. Use Arrow Functions to Write Concise Anonymous Functions
 

    ```js
    const magic = () => {
    "use strict";
    return new Date();
    };
    
    ```

5. Write Arrow func with parameters:-

    ```js
    const myConcat = (arr1, arr2) =>  {
    return arr1.concat(arr2);
    };

    console.log(myConcat([1, 2], [3, 4, 5]));

    ```

6. Set Default Parameters for Your Functions

    ```js

    function increment(number, value = 1) {
        return number + value;
    }
    console.log(increment(5, 2)); // returns 7
    console.log(increment(5)); // returns NaN

    ```

7. Set Default Parameters for Your Functions:-

    ```js

    function increment(number, value = 1) {
        return number + value;
    }
    console.log(increment(5, 2)); // returns 7
    console.log(increment(5)); // returns NaN

    ```

8. Use the Rest Parameter with Function Parameters:-

    ```js
    const sum = (...args) => {
    let total = 0;
    for (let i = 0; i < args.length; i++) {
        total += args[i];
    }
    return total;
    }

    ```

9. Use the Spread Operator to Evaluate Arrays In-Place

    ```js

   const arr1 = ['JAN', 'FEB', 'MAR', 'APR', 'MAY'];
    let arr2;
    (function() {
    "use strict";
    arr2 = [...arr1]; // change this line
    })();
    console.log(arr2);

    ```

10. Use Destructuring Assignment to Extract Values from Objects

    ```js
    const HIGH_TEMPERATURES = {
    yesterday: 75,
    today: 77,
    tomorrow: 80
    };

    // change code below this line

    const {today, tomorrow} = HIGH_TEMPERATURES;

    // change code above this line


    console.log(today); // should be 77
    console.log(tomorrow); // should be 80

    ```

11. Use Destructuring Assignment to Assign Variables from Objects

    ```js
    const HIGH_TEMPERATURES = {
    yesterday: 75,
    today: 77,
    tomorrow: 80
    };

    const { today: highToday, tomorrow: highTomorrow } = HIGH_TEMPERATURES;

    ```

12. Use Destructuring Assignment to Assign Variables from Nested Objects

    ```js
    const LOCAL_FORECAST = {
    yesterday: { low: 61, high: 75 },
    today: { low: 64, high: 77 },
    tomorrow: { low: 68, high: 80 }
    };
    
    const { today: { low: lowToday, high: highToday }} = LOCAL_FORECAST;

    ```

13. Use Destructuring Assignment to Assign Variables from Arrays

    ```js
    let a = 8, b = 6;
    // change code below this line
    [a,b] = [b,a];
    // change code above this line
    console.log(a); // should be 6
    console.log(b); // should be 8

    ```

14. Destructuring via rest elements

    ```js
    function removeFirstTwo(list) {
    // Only change code below this line
    const [a, b, ...shorterList] = list; // Change this line
    // Only change code above this line
    return shorterList;
    }

    const source = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
    const sourceWithoutFirstTwo = removeFirstTwo(source);

    ```

15. Use Destructuring Assignment to Pass an Object as a Function's Parameters

    ```js
    const stats = {
    max: 56.78,
    standard_deviation: 4.34,
    median: 34.54,
    mode: 23.87,
    min: -0.75,
    average: 35.85
    };
    // change code below this line
    const half = ({max, min}) => ((max + min) / 2.0); // use function argument destructurung
    // change code above this line
    console.log(stats); // should be object
    console.log(half(stats)); // should be 28.015

    ```
    
16. Create Strings using Template Literals

    ```js
    const result = {
    success: ["max-length", "no-amd", "prefer-arrow-functions"],
    failure: ["no-var", "var-on-top", "linebreak"],
    skipped: ["no-extra-semi", "no-dup-keys"]
    };
    function makeList(arr) {
    "use strict";
    // change code below this line
    const failureItems = [];
    for (let i = 0; i < arr.length; i++) {
        failureItems.push(`<li class="text-warning">${arr[i]}</li>`);
    }
    // change code above this line
    return failureItems;
    }

    const failuresList = makeList(result.failure);

    ```

17. Write Concise Object Literal Declarations Using Object Property Shorthand

    ```js
    // change code below this line
    const createPerson = (name, age, gender) => {
    return {name,age,gender};
    };
    // change code above this line
    console.log(createPerson("Zodiac Hasbro", 56, "male")); // returns a proper object

    ```

        

            
                