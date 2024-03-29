# Application Architecture, MVC Design Pattern
01. What are the Pillars of Object Oriented Programming (`OOP`)?
  
  > | The four pillars of object-oriented programming (OOP) are encapsulation, inheritance, polymorphism, and abstraction. By using these four pillars of OOPs, developers can create programs that are powerful, maintainable, and extensible, making them a great choice for software development. |

02. How does `export` differ from `export default`?
  
  > | Use named export when you want to export multiple variables or functions from a file. Use default export when you want to export only one variable or function from a file. Use named export when you want to keep the same name for your variables or functions across different files. |

03. What is Encapsulation?
  
  > | Encapsulation describes bundling data and methods that work on that data within one unit. We often use this concept to hide an object’s internal representation or state from the outside. This is called information hiding. The general idea of this mechanism is simple. For example, you have an attribute that is not visible from the outside of an object. You bundle it with methods that provide read or write access. Encapsulation allows you to hide specific information and control access to the object’s internal state. |

04. What are some of the benefits of the `Proxy` object that we are using in our structure for applications?
  
  > | The Proxy object allows you to create an object that can be used in place of the original object, but may redefine fundamental Object operations like getting, setting, and defining properties. Proxy() provides an interface to control the behavior of any target object using handler and trap, users can balance among simplicity and utility of an object. In ES6 Proxy offers the flexibility of eating your cake and having it back. |

05. What the difference between a `class` and an instance of a `class`?
  
  > | The class = the blue print. The object is an actual thing that is built based on the 'blue print' (like the house). An instance is a virtual copy (but not a real copy) of the object. A blueprint for a house design is like a class description. All the houses built from that blueprint are objects of that class. A given house is an instance. |

06. What is a computed Property?
  
  > | Computed properties are like data properties, except they depend on other properties. A computed property automatically tracks its reactive dependencies. Computed properties are written like methods, but they do not accept any input arguments. |

07. What is the purpose of the `MVC` pattern?
  
  > | The actual purpose of MVC is to separate your views from your controller and model. In other words, it is a design pattern in a structure for keeping display and data separate to allow each to change without affecting the other. A design pattern prevents the problems and difficulties of spaghetti code. |

08. What is the job of the `Controller` in the `MVC` Pattern?
  
  > | The controller's responsibility is to pull, modify, and provide data to the user. Essentially, the controller is the link between the view and model. Through getter and setter functions, the controller pulls data from the model and initializes the views. |

09. What is the job of the `Service` in `MVC`?
  
  > | The service layer is an additional layer in an application that mediates communication between a controller and repository layer. The service layer contains business logic. In particular, it contains validation logic. |

10. What is the job of the `Model` in `MVC`?
  
  > | The backend that contains all the data logic. Whether the data is from a database, API, or a JSON object, the model is responsible for managing it. |
