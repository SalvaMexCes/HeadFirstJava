# HeadFirstJava

//CHAPTER 3

  -Primitive type / Value Range
  -char / 0 to 65535
  -byte / -128 to 127
  -short / -32768 to 32767
  -int / -2147483648 to 2147483647
  -long / -huge to huge
  -float / varies
  -double / varies

  -"Although a PRIMITVE variable is full of bits representing the actual 'value' of the variable, an OBJECT reference variable is full of bits representing 'a way to get to the object'."
  -You use the dot operator (.) on a reference variable to say "use the thing before the dot to get me the thing after the dot".
  -Variables are always declared with a name and a type.
  -A reference variable value is the bits representing a way to get to an object on the heap.
  -A reference varaibble has a value of "null" when it is not referencing any object.
  -An arrays is ALWAYS an object.

  -      1          2
  -  Dog myDog = new Dog();
  - 1) Declare a reference value
    2) Create an object

       
  - int array variable = " int[] nums; "
  - A new array with a length of 7, and assigned to previous int[] variable
  - nums = new int[7];





//Chapter 4

- Every instance of a particular class has the same methods, but the methods can behave differently based on the value of the instance variables.
- Classes define what an object knows and what an object does.
- Things a class knows are INSTANCE VARIABLES. Things a class does are its METHODS.
- When using methods, you MUST pass it values of the appropriate type.
- Methods with a "void" return type don't give anything back.
- But you can declare a method to give a specific type of value back to the caller. But you MUST return a value of the declared type.
- Methods have multiple parameters, meaning you can send more than one thing to a method, but you MUST pass arguments of the right type and order.
- An encapsulation starter rule of thumb is to: mark your instance variables PRIVATE and provide PUBLIC getters and setters for access control.
- INSTANCE VARIABLES are declared inside a class but not within a method.
- LOCAL VARIABLES are declared within a method. MUST be initiaalized before use.
- Use the "==" operator to compare if two primitives are equal(the same).
- The "==" operator can also compare two variables of any kind and any two references.





//Chapter 7

- When talking about OOP's, There are SUPERCLASSES and SUBCLASSES
- A Superclass holds the main method while Subclasses hold the custom methods.
- "The subclass INHERITS from the superclass".
- Subclasses can have the same instance variables but different values.
- When you call a method on an object reference, you're calling the most specific version of the method for that object type. In other words "The lowest one wins", lowest meaning lowest on the inheritance tree.
- If a class inherits a method, it HAS the method.
- The inheritance "IS-A" relationship hiearchy only works in ONE DIRECTION.
- Inherited methods can be overided, instance variables cannot.
- A superclass can  never know what's in the subclasses.
- A superclass can choose what to and what NOT to pass onto its subclasses, by the level of access (PRIVATE, DEFAULT, PROTECTED & PUBLIC).
- Access levels control who sees what. CRUCIAL to having well designed java code.
- DO use inheritance when one class is a more specific type of a superclass.
- DO consider inheritance when you have behavior (implemented code) that should be shared among multiple classes of the same type.
- DO NOT use inheritance so that you can reuse code from another class, if the relationship between subclasses violate either of the above two rules.
- DO NOT use inheritance is the subclass and superclass do not pass the "IS-A" test.
- AVOID DUPLICATE CODE by putting common code in one place and let the subclasses inherit it.
- When you define a supertype for a group of classes, any subclass of that supertype can be substituted where the supertype is expected.
- This allows to write really flexible code.
- With POLYMORPHISM, the reference and the object can be different.
- Anything that extends the declared reference type can be assigned to the reference variable.
- With polymorphism, you can write code that doesn't have to change when you introduce new subclass types into the program.
- The arguments and return types of your overriding method must look to the outside world EXACTLY like the overriden method in the superclass.
- You CANNOT change the arguments in an overriding method.
- Whatever the superclass takes as an argument, the subclass overriding the method MUST use that same argument.
- Whatever the superclass declares as a return type, the overriding method must declare either the same type, or a subclass type.
- This also means ACCESS LEVELS must be the same, or friendlier.
- METHOD OVERLOADING is nothing more than having two methods with the same name but different argument lists.
- An overloaded method is just a different method with the same name.
- There's no polymorphism involved with overloaded methods.
- Overloading lets you make multiple versions of a method, with different argument lists, for convenience to the callers.
- With overloaded methods, you can have different return types, and you can vary the access levels in any direction.
- YOU CAN'T CHANGE ONLY THE RETURN TYPE (if only the return type is different, it is NOT an overloaded method. 













