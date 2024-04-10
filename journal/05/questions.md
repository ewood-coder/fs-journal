# Intro to Server side concerns with JavaScript
01. What do the letters of the acronym `CRUD` stand for?

  > | The acronym stands for Create, Read, Update, and Delete representing the four main operations performed on data. CRUD is a foundational concept in computer programming, databases, and application design. |

02. Each action that `CRUD` represents maps to an HTTP request. What HTTP request does each `CRUD` action correspond to?

  > | Create = post, Read = get, Update = put, Delete = delete |

03. What does `ORM` stand for? Which `ORM` do we use when interacting with MongoDB

  > | ORM stands for Object-relational Mapper. ORMs are software tools that help developers interact with relational databases by translating between the data representations used by databases and those used in object-oriented programming. The ORM we are using with MongoDB is mongoose. |

04. Which two `HTTP` request types include a body?

  > | Post & Put. The POST method is used to send data to a server to create a new resource. In the context of CRUD operations in REST APIs: Create: It is used for the "Create" operation. PUT is the HTTP method used for the CRUD operation, Update. For example, if the price of Avocado Toast has gone up, we should go into the database and update that information. We can do this with a PUT request. |

05. In a/an _______ coding model, when you call a function, it returns only when the action has finished and stops your program for the time the action takes. Likewise in a/an _______ coding model, multiple things are allowed to happen at one time. When you perform an action, your program continues to run.  Fill in the blanks.

  > | 1. Synchronous     2. Asynchronous |

06. What are the three types of data relationships? Provide an example of each.

  > | One-to-one: For example, in a school database, each student has only one student ID, and each student ID is assigned to only one person. One-to-many: For example, one customer (in a customers table) having many orders (in an orders table). Many-to-many: For example, a student can enroll in multiple courses, and each course can have multiple students enrolled. |

07. What is middleware?

  > | Middleware is a type of computer software program that provides services to software applications beyond those available from the operating system. It can be described as "software glue".  |

08. The ______ pipeline delivers information from the client while the ______ pipeline returns it. Fill in the blanks. 

  > | The request pipeline delivers information from the client while the response pipeline returns it. |

09. Demonstrate the pattern that is used to include a request query with the client's `HTTP` request providing the property `tag` and the value `winter`.

  > | http://localhost:3000/api/jobs/?tag=winter    OR    const response = await dbContext.jobs.find({"tag": "winter"}) |

10. What is a ***virtual property***?

  > | Virtual properties are small javascript functions (called formulas) that can be used to create properties based on values stored in an element or in the elements in its neighborhood. This formula has to return a single value (string or number) which represents the value of this virtual property for the particular element. |
