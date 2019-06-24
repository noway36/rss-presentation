1. Hello. My name is Alexander and today we are going to talk about TypeScript. So if you're confused what Typescript is and why do we use it, when we already have javascript available which is fulfilling all our needs, then I will try to answer all these questions.

2. So. What TypeScript is? By definition, “TypeScript is JavaScript for application-scale development”. TypeScript is both a language and a set of tools. It was designed to develop large Javascript applications. TS helps us write stable code. Everyone loves stable code, thats why we need TS.

2.1. In other words Typescript is a superset of Javascript. It means you don’t have to worry about converting the whole existing Javascript code into Typescript at once. Instead if you wish to migrate your existing Javascript code to Typescript, you can do that gradually.

2.2. TypeScript was launched for public use in October 2012.It was a result of two years of developing at Microsoft, with Anders Hejlsberg, also known as lead architect of C#. Next we will see that TS have a lot in common with C#.

3. First of all, we have to understand, that TypeScript is just JavaScript. Typescript adopts the basic building blocks of your program from JavaScript. Hence, you only need to know JavaScript to use TypeScript. All TypeScript code is converted into its JavaScript equivalent for the purpose of execution.

TypeScript supports other JS libraries. TypeScript-generated JavaScript can reuse all of the existing JavaScript frameworks, tools, and libraries.

JavaScript is TypeScript. This means that any valid .js file can be renamed to .ts and compiled with other TypeScript files.

TypeScript is portable across browsers, devices, and operating systems. It can run on any environment that JavaScript runs on. TypeScript doesn’t need a dedicated VM or a specific runtime environment to execute.

4. There are some major benefits of using Typescript, which includes, support for Classes and Modules, Type-checking, ES6 features support, supports OOP concepts(like interfaces, inheritance, etc.), and a lot more.

5. Now let's talk about type system in TS. As we know JS is a weakly typed language, meaning you don’t have to specify what type of information will be stored in a variable.
   While JavaScript’s type system gives you a lot of flexibility, it lacks the capability of a strongly typed system, which protects you from spending hours debugging a type error.

5.0 In that simple example we won't get the type error, but there is unexpexted behavior of function sum, which should return a number. By the way we can even invoke that function with two objects and get the string value back.
TypeScript can help us to deal with that trouble by fixing values that function takes and returns.

5.1 Here we can see TS version of that function.

5.2 And now let's consider TS syntax. TypeScript supports much the same types as we would expect in JavaScript. Here is some examples of TS syntax for primitive data types: number string, boolean, null, undefined.
We are literally saying that in the variable num we must store a number type value, in variable bool we should store a boolean type value and so on.

5.3 TypeScript provides dedicated type syntax for arrays to make it easier for you to annotate and document your code. It allows you to safely do any array manipulation that you would normally do and protects you from errors like assigning a member of the wrong type.

5.4 Tuple type allows you to express an array where the type of a fixed number of elements is known, but need not be the same.

5.5 Interfaces are the core way in TypeScript to compose multiple type annotations into a single named annotation. Interfaces have zero runtime JavaScript impact. There is a lot of power in TypeScript interfaces to declare the structure of variables.
Properties with question mark next to it are optional.

5.6 We may need to describe the type of variables that we do not know when we are writing an application. In that case we use "any" type. The any type is also handy if you know some part of the type, but perhaps not all of it. For example, you may have an array but the array has a mix of different types.
Void is a little like the opposite of any: the absence of having any type at all. You may commonly see this as the return type of functions that do not return a value. Declaring variables of type void is not useful because you can only assign undefined or null to them.

5.7 If you want to use classes that must follow an object structure that someone declared for you in an interface you can use the implements keyword to ensure compatibility

6. Now I want to tell you more about OOP concepts in TypeScript.
   Traditional JavaScript uses functions and prototype-based inheritance to build up reusable components, but this may feel a bit awkward to programmers more comfortable with an object-oriented approach, where classes inherit functionality and objects are built from these classes. TypeScript allows developers to build their applications using this object-oriented class-based approach.

6.1 Let’s take a look at a simple class-based example.
The syntax should look familiar if you’ve used C# or Java before. We declare a new class Greeter. This class has three members: a property called greeting, a constructor, and a method greet.
You’ll notice that in the class when we refer to one of the members of the class we prepend this dot. This denotes that it’s a member access.

6.2 In TypeScript, we can use common object-oriented patterns. One of the most fundamental patterns in class-based programming is being able to extend existing classes to create new ones using inheritance. This example shows the most basic inheritance feature: classes inherit properties and methods from base classes. Here, Dog is a derived class that derives from the Animal base class using the extends keyword. Derived classes are often called subclasses, and base classes are often called superclasses.
Because Dog extends the functionality from Animal, we were able to create an instance of Dog that could both bark() and move().

6.3 If you’re familiar with classes in other languages, you may have noticed in the above examples we haven’t had to use the word public to accomplish this; for instance, C# requires that each member be explicitly labeled public to be visible. In TypeScript, each member is public by default.
You may still mark a member public explicitly. We could have written the Animal class from the previous section in the following way.

6.4 When a member is marked private, it cannot be accessed from outside of its containing class.

6.5 The protected modifier acts much like the private modifier with the exception that members declared protected can also be accessed within deriving classes. Notice that while we can’t use name from outside of Person, we can still use it from within an instance method of Employee because Employee derives from Person.

6.6 In TypeScript 2, the readonly modifier was added to the language. Properties marked with readonly can only be assigned to during initialization or from within a constructor of the same class. All other assignments are disallowed.

6.7 We can also create static members of a class, those that are visible on the class itself rather than on the instances. In this example, we use static on the origin, as it’s a general value for all grids. Each instance accesses this value through prepending the name of the class. Similarly to prepending this. in front of instance accesses, here we prepend Grid. in front of static accesses.

6.8 Abstract classes are base classes from which other classes may be derived. They may not be instantiated directly. Unlike an interface, an abstract class may contain implementation details for its members. The abstract keyword is used to define abstract classes as well as abstract methods within an abstract class.

7. Here are some links that you may find useful.

8. So. That's all I wanted to tell you about TS. TypeScript is kinda big topic to talk about, but I hope I answered all the questions that were asked at the beginning of that presentation. Thank you for watching.
