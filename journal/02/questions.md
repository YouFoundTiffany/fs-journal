# Intro to JavaScript
01. Which keywords are used to declare a variable in JavaScript?

    > let var const

02. What is the definition of a function?

    > A function is a subprogram designed to perform a particular task.


03. What are the `SOLID` principles?

    SOLID principles are object-oriented design concepts relevant to software development. SOLID is an acronym for five other class-design principles: Single Responsibility Principle, Open-Closed Principle, Liskov Substitution Principle, Interface Segregation Principle, and Dependency Inversion Principle.

04. Given this array: How could you remove the `pineapple`?
I believe you could use at least two options for finding pineapple, a find or forEach method.
    ```js
    let fruit = ['apple', 'banana', 'pineapple', 'orange', 'strawberry']
    > let findP = fruit.find((pineapple) => pineapple === 'pineapple');
console.log(findP)



    The find() method of Array instances returns the first element in the provided array that satisfies the provided testing function. If no values satisfy the testing function, undefined is returned.

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
    ```

    > | ANSWER HERE |

06. Give an example of a JavaScript `Conditional`:

    > let num1 = 10 , or if (num1 > num2) 

07. What is the main difference between `parameters` and `arguments`?

    > A parameter is a variable in a function definition. It is a placeholder and hence does not have a concrete value. An argument is a value passed during function invocation.

08. Instead of writing everything to the console, what is a better way to debug your code?

    > Use the debugger in your function to go through it step by step to see what elements and values are correct or incorrect. The Sources tab, which allows you to view all of your source files, add breakpoints in your code, and debug your code line by line.

09. What is the difference between a `primitive` value and a `reference` value?

    > Numbers, boolean values, and the null and undefined types are primitive. Objects, arrays, and functions are reference types.

10. Demonstrate a loop that prints the numbers between -100 and 100?

    > for (let number = -100; number <= 100; number++) {
    console.log(number)
}
