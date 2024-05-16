# CSharp and SQL Fundamentals
01. What is the purpose of a `namespace`?

  > | Namespaces are used to organize code into logical groups and to prevent name collisions that can occur especially when your code base includes multiple libraries. All identifiers at namespace scope are visible to one another without qualification. |

02. What is the difference between a `class` and an `interface`?

  > | The main distinction between a class and an interface is that a class will be used to describe the behavior of the objects in the program, whereas an interface will carry those behaviors. |

03. What is the method that returns an instance of a class, yet it has no return type?

  > | A void method doesn't return any value, the only point of calling one is because it does something that can be observed by the user or by other code. It changes the state of the object or maybe causes something to happen like drawing a line on the screen. |

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

  > | 'public' is the answer. Access modifiers in C# are used to specify the scope of accessibility of a member of a class or type of the class itself. For example, a public class is accessible to everyone without any restrictions, while an internal class may be accessible to the assembly only. |

06. In the Car example what is `string` an indication of?

  > | String indicates that whatever is going to returned in that function will be a string. |

07. In the Car example what is `abstract` preventing?

  > | The abstract class is a restricted class that cannot be used to create objects (to access it, it must be inherited from another class). It is preventing class Car from being able to create objects. |

08. In a SQL table, what is the difference between information in a row and information in a column?

  > | A row is a horizontal alignment of data, while a column is vertical. Data in a row contains information that describes a single entity, while data in a column describes a field of information all entities possess. |

09. Demonstrate the necessary SQL for creating a table called `characters` with the values `name, age, description` as strings, and an `int` id.

  > CREATE TABLE characters (
  > 	id INT NOT NULL AUTO_INCREMENT PRIMARY KEY,
  > 	name VARCHAR(255) NOT NULL,
  > 	age VARCHAR(255) NOT NULL, (why would age be a string? I dunno)
  > 	description VARCHAR(5000) NOT NULL
  > );

10. In SQL how can you query more than a single table? Provide an example.

  > SELECT department.ID, department.NAME, employee.Email, employee.City FROM department, employee 
  > WHERE department.ID = employee.ID;

  > OR

  > SELECT * FROM department, employee
