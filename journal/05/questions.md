# Intro to Server side concerns with JavaScript
01. What do the letters of the acronym `CRUD` stand for?

  > | Create, Read, Update, Delete |

02. Each action that `CRUD` represents maps to an HTTP request. What HTTP request does each `CRUD` action correspond to?

  > | Post, Get, Put, Delete |

03. What does `ORM` stand for? Which `ORM` do we use when interacting with MongoDB

  > | Object relational mapping, express and node |

04. Which two `HTTP` request types include a body?

  > | Post and Put |

05. In a/an _______ coding model, when you call a function, it returns only when the action has finished and stops your program for the time the action takes. Likewise in a/an _______ coding model, multiple things are allowed to happen at one time. When you perform an action, your program continues to run.  Fill in the blanks.

  > | Async and sync |

06. What are the three types of data relationships? Provide an example of each.

  > | one to one - a relationship between two entities when an object only has one relation, like 1 owner and 1 house is a 1 to 1.
      one to many- a relationship where one side can have many relations for example 1 owner and 3 houses.
      many to many- a relationship where both sides have many relations for example 3 owners and 6 houses. |

07. What is middleware?

  > | A middle man that works between an application and a database, used to communicate between the both of them. |

08. The ______ pipeline delivers information from the client while the ______ pipeline returns it. Fill in the blanks. 

  > | Request, Response |

09. Demonstrate the pattern that is used to include a request query with the client's `HTTP` request providing the property `tag` and the value `winter`.

  > | .get(tag/winter), this.whatever |

10. What is a ***virtual property***?

  > | Virtual properties are additional properties to a model that don't get stored in database they only exist logically |
