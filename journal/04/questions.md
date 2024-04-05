# Understanding Asynchronous Code, and API's
01. What is the difference between `asynchronous` code and `synchronous` code?

  > | The differences between asynchronous and synchronous include: Async is multi-thread, which means operations or programs can run in parallel. Sync is a single-thread, so only one operation or program will run at a time. Async is non-blocking, which means it will send multiple requests to a server. |

02. What is an event listener?

  > | An event listener is a function in JavaScript that waits for an event to occur then responds to it. JavaScript’s event listener function allows you to create custom responses to events like mouse clicks, keyboard clicks, and window resizing. The programming paradigm of waiting and responding to real-time events is called event handling. |

03. What does *REST* stand for, and in simple terms what does it mean??

  > | REST (REpresentational State Transfer) is an architectural style for developing web services and systems that can easily communicate with each other. In simpler words, it is a software architecture that imposes conditions on how an API should work. |

04. What is a callback / higher order function?

  > | A function that accepts a function as an argument and/or returns a function as its value. |

05. What is a `promise`? How do you capture an error from a `promise`?

  > | an object that will produce a single value some time in the future. If the promise is successful, it will produce a resolved value, but if something goes wrong then it will produce a reason why the promise failed. To handle any errors that may occur in the chain, you can add a call to catch at the end of the chain. If any of the promises are rejected, this catch handler will run, and the rest of the chain is skipped. |

06. Name three processes used to make requests over `HTTP`?

  > | GET: The GET method requests a representation of the specified resource, POST: The POST method submits an entity to the specified resource, often causing a change in state or side effects on the server, PUT: The PUT method replaces all current representations of the target resource with the request payload. |

07. What does the `API` acronym stand for?

  > | API stands for Application Programming Interface. In the context of APIs, the word Application refers to any software with a distinct function. Interface can be thought of as a contract of service between two applications. This contract defines how the two communicate with each other using requests and responses. |

08. What must you do in order to `await` a promise inside of a function?

  > | You must put async before the function name and place await in front of the HTTP request. |

09. What is the purpose of encapsulation in programming?

  > | Encapsulation is a way to restrict the direct access to some components of an object, so users cannot access state values for all of the variables of a particular object. Encapsulation can be used to hide both data members and data functions or methods associated with an instantiated class or object. |

10. What is `HTTP` response code for a successful request?

  > | The 200 OK status code means that the request was successful, but the meaning of success depends on the request method used: GET: The requested resource has been fetched and transmitted to the message body. |

11. What is a 400 error?

  > | A 400 error, also known as a "Bad Request" error, is an HTTP response status code that indicates that a browser sent a request to a web server that the server cannot understand or process correctly. This error is related to the submitted request from the client before it is even processed by the server. HTTP status codes starting with 4XX typically indicate an error on the client side. |
