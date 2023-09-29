# Intro to JavaScript
01. Which keywords are used to declare a variable in JavaScript?

    > | Let, var and const |

02. What is the definition of a function?

    > | a subprogram designed to perform a particular task |

03. What are the `SOLID` principles?

    > | Single responsible principle (srp)
    Open closed principle (ocp)
    Liskov substitute principle (lsp)
    Interface segregation principle (isp)
    Dependency inversion principle (dip)
     |

04. Given this array: How could you remove the `pineapple`?

    ```js
    let fruit = ['apple', 'banana', 'pineapple', 'orange', 'strawberry']
    ```

    > | fruit.splice(2,1); |

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

    > | const friends = [
    {
        name: 'bob'
    },

    {
        name: 'joe'
    }
]

let you = {
    name: "You",
    hair: true,
    friends: [friends]
}
let them = {
    name: "Them",
    hair: false,
    friends: [friends]
} |

06. Give an example of a JavaScript `Conditional`:

    > | If(bob >= joe){
        return true
    } else{
        return false
    } |

07. What is the main difference between `parameters` and `arguments`?

    > | Parameters are variables declared inside of a function and arguments are the values of the variable that gets passed to the function |

08. Instead of writing everything to the console, what is a better way to debug your code?

    > | Using the developer tools |

09. What is the difference between a `primitive` value and a `reference` value?

    > | Primitive values are values stored independently outside of a function and Reference values are values stored inside a function that are called within that specific function only. |

10. Demonstrate a loop that prints the numbers between -100 and 100?

    > | for(let i = -100; i <= 100; i++){
        console.log (i)
    } |
