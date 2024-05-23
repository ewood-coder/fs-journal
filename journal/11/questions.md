# A bit more CSharp and SQL
1. What does ***inheritance*** accomplish for us in C#?

  > | Inheritance, in C#, is the ability to create a class that inherits attributes and behaviors from an existing class. The newly created class is the derived (or child) class and the existing class is the base (or parent) class. |

2. How does ***member inheritance*** work in C#? Does a `Class` inherit all members of the base `Class`?

  > | In C#, member inheritance allows derived classes (child classes) to inherit members (fields, properties, methods, etc.) from their base class (parent class). This enables the child class to access and use the members defined in the base class without redefining them. When a class inherits from another class, it doesn't automatically inherit all members of the base class. Instead, it inherits all accessible members of the base class, which typically includes public and protected members. Private members of the base class are not directly accessible to the derived class. |

3. How does ***accessibility*** affect inheritance?

  > | While all other members of a base class are inherited by derived classes, whether they are visible or not depends on their accessibility. A member's accessibility affects its visibility for derived classes as follows: private, protected, internal, and public. |

4. What is the difference between a `PRIMARY KEY` and a `FOREIGN KEY`

  > | A primary key is a unique identifier for each record in a table. A foreign key establishes a relationship between tables by referencing the primary key of another table. Ensures uniqueness and data integrity within a single table. Establishes relationships and maintains referential integrity between tables. |

5. What is an ***alias***?

  > | In C#, an alias is a way to provide alternative names for types, namespaces, or assemblies. This feature is particularly useful when you have long or cumbersome names that you need to use frequently, or when you want to avoid naming conflicts. There are two main types of aliases in C#: type alias & namespace alias. |

6. Demonstrate how you would query a join statement that would get all of a doctors patients from the following collections:

  ```SQL
  CREATE TABLE doctors (
    id INT NOT NULL AUTO_INCREMENT,
    -- CODE OMITTED
    PRIMARY KEY (id)
  )

  CREATE TABLE patients (
    id INT NOT NULL AUTO_INCREMENT,
    -- CODE OMITTED
    PRIMARY KEY (id)
  )

  CREATE TABLE patient_doctors (
    id INT NOT NULL AUTO_INCREMENT,
    doctorId INT NOT NULL,
    patientId INT NOT NULL,

    FOREIGN KEY (doctorId)
      REFERENCES doctors(id),
    FOREIGN KEY (patientId)
      REFERENCES patients(id),
  )

  ```

  > SELECT *
  > FROM patients
  > JOIN patient_doctors ON patients.id = patient_doctors.patientId
  > JOIN doctors ON patient_doctors.doctorId = doctors.id
  > WHERE doctors.id = patient_doctors.doctorId;
