# Intro to JavaScript
01. Which keywords are used to declare a variable in JavaScript?

    > | Var, let and const. Var declarations are globally scoped or function scoped while let and const are block scoped. Var variables can be updated and re-declared within its scope; let variables can be updated but not re-declared; const variables can neither be updated nor re-declared. They are all hoisted to the top of their scope but while var variables are initialized with undefined, let and const variables are not initialized. While var and let can be declared without being initialized, const must be initialized during declaration. |

02. What is the definition of a function?

    > | A function is a subprogram designed to perform a particular task. Functions are executed when they are called. This is known as invoking a function. Values can be passed into functions and used within the function. Functions always return a value. The name of the value is called a parameter and the actual value itself is called an argument. In JavaScript, if no return value is specified, the function will return undefined. Functions are objects. A Function Declaration defines a named function. To create a function declaration you use the function keyword followed by the name of the function. When using function declarations, the function definition is hoisted, thus allowing the function to be used before it is defined. |

03. What are the `SOLID` principles?

    > | SOLID is a mnemonic acronym for five design principles intended to make object-oriented designs more understandable, flexible, and maintainable.                                       																												S: Single-responsibility Principle    																																	O: Open-closed Principle 																																					L: Liskov Substitution Principle 																																		I: Interface Segregation Principle  																																	D: Dependency Inversion Principle |

04. Given this array: How could you remove the `pineapple`?

    ```js
    let fruit = ['apple', 'banana', 'pineapple', 'orange', 'strawberry']
    ```

    > | There are a few ways I could remove pineapple from the array. These include the DELETE operator, the splice() method, and a slightly longer way: the filter() method 																																											const myArray = ['apple', 'banana', 'pineapple', 'orange','strawberry']; 																				const x = myArray.splice(2, 1); 																					  												 console.log(`myArray values: ${myArray}`); 																														console.log(`variable x value: ${x}`); 																															THIS WILL DISPLAY ALL THE VALUES NOT REMOVED IN THE ARRAY AND STORE THE REMOVED VALUE ELSEWHERE |

05. Given these two objects: How could you add each to the others friends arrays?

    ```js
    let you = {
        name: "You",
        hair: true,
        friends: []
    }
    let them = {
        name: "Them",
        hair: false,
        friends: []
    }

	 you.friends.push(them.name); //remove the .name if you want to add all properties for the array
	 them.friends.push(you.name); //remove the .name if you want to add all properties for the array

	 console.log(you.friends); // logs: {"Them"}
	 console.log(them.friends); // logs: {"You"}
    ```

    > | Answer is included in the showcase of the code |

06. Give an example of a JavaScript `Conditional`:

    > | There are multiple conditionals such as if, else, else if, and switch statements.            ex/ if (hour < 18) { greeting = "Good day"; } |

07. What is the main difference between `parameters` and `arguments`?

    > | Parameters are used when defining a function, they are the names created in the function definition. Parameters are separated by commas in the (). Arguments, on the other hand, are the values the function receives from each parameter when the function is executed (invoked).|

08. Instead of writing everything to the console, what is a better way to debug your code?

    > | You can use the debugger statement in JavaScript to debug your code effectively. This will allow you to pause the execution and inspect the variables at that point. |

09. What is the difference between a `primitive` value and a `reference` value?

    > | In programming, the main difference between a primitive value and a reference value lies in how they are stored and accessed in memory. In simpler terms, primitive values are stored directly with their own unique memory location, while reference values store a memory address that points to the actual location of the data. Primitive values are simple data types like numbers, strings, booleans, null, and undefined. Reference values are more complex data types like objects and arrays. |

10. Demonstrate a loop that prints the numbers between -100 and 100?

    > | for (let i = -100; i <= 100; i++) { console.log(i); } |
