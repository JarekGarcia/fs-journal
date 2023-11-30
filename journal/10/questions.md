# CSharp and SQL Fundamentals
01. What is the purpose of a `namespace`?

  > | its pretty much like import/export so when you declare a namespace you are using that export that is usually in the globals |

02. What is the difference between a `class` and an `interface`?

  > | A class specifies how to create and use object of that type and interface is a set of rules that describes what an object can do but has no implementation of how it works. |

03. What is the method that returns an instance of a class, yet it has no return type?

  > | VOID |

05. In the Car example what is the access modifier of the `Start()` method?

  ```c#
  abstract class Car
  {
    public string Start()
    {

      return "Vroooom";

    }
  }
  ```

  > | Public which means it can be used again in the same class and outside if referenced |

06. In the Car example what is `string` an indication of?

  > | It is the return type so it returns the string "Vroooom" |

07. In the Car example what is `abstract` preventing?

  > | Its preventing an instance of that class it can only be inherited by other instances as a base |

08. In a SQL table, what is the difference between information in a row and information in a column?

  > | rows contain unique records of data and the column represents the field or category of data |

09. Demonstrate the necessary SQL for creating a table called `characters` with the values `name, age, description` as strings, and an `int` id.

  > | CREATE TABLE IF NOT EXISTS characters(
    id INT NOT NULL PRIMARY KEY AUTO_INCREMENT,
    name CHAR(50) NOT NULL,
    age CHAR(50) NOT NULL,
    description CHAR(255) NOT NULL
  ) default charset utf8 COMMENT''; |

10. In SQL how can you query more than a single table? Provide an example.

  > | You can use join to query from multiple tables so lets say you have two tables example1 and example2 you can do this.
  SELECT * example1 JOIN example2
  this will join everything because we selected all by using * and it will join both tables together in one.  |
