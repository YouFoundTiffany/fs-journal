# A bit more CSharp and SQL
1. What does ***inheritance*** accomplish for us in C#?

  >  code reuse, hierarchy, and specialization

2. How does ***member inheritance*** work in C#? Does a `Class` inherit all members of the base `Class`?

  >Inheritance is one of the fundamental attributes of object-oriented programming. It allows you to define a child class that reuses (inherits), extends, or modifies the behavior of a parent class. The class whose members are inherited is called the base class. The class that inherits the members of the base class is called the derived class.

C# and .NET support single inheritance only. That is, a class can only inherit from a single class. However, inheritance is transitive, which allows you to define an inheritance hierarchy for a set of types. In other words, type D can inherit from type C, which inherits from type B, which inherits from the base class type A. Because inheritance is transitive, the members of type A are available to type D.

Not all members of a base class are inherited by derived classes. The following members are not inherited:

Static constructors, which initialize the static data of a class.

Instance constructors, which you call to create a new instance of the class. Each class must define its own constructors.

Finalizers, which are called by the runtime's garbage collector to destroy instances of a class.

Static constructors, which initialize the static data of a class.

Instance constructors, which you call to create a new instance of the class. Each class must define its own constructors.

Finalizers, which are called by the runtime's garbage collector to destroy instances of a class.

3. How does ***accessibility*** affect inheritance?

  > While all other members of a base class are inherited by derived classes, whether they are visible or not depends on their accessibility. A member's accessibility affects its visibility for derived classes as follows:

Private members are visible only in derived classes that are nested in their base class. Otherwise, they are not visible in derived classes. In the following example, A.B is a nested class that derives from A, and C derives from A. The private A._value field is visible in A.B. However, if you remove the comments from the C.GetValue method and attempt to compile the example, it produces compiler error CS0122: "'A._value' is inaccessible due to its protection level."

Protected members are visible only in derived classes.

Internal members are visible only in derived classes that are located in the same assembly as the base class. They are not visible in derived classes located in a different assembly from the base class.

Public members are visible in derived classes and are part of the derived class' public interface. Public inherited members can be called just as if they are defined in the derived class. In the following example, class A defines a method named Method1, and class B inherits from class A. The example then calls Method1 as if it were an instance method on B.

4. What is the difference between a `PRIMARY KEY` and a `FOREIGN KEY`

  > A primary key is used to ensure data in the specific column is unique.	A foreign key is a column or group of columns in a relational database table that provides a link between data in two tables.

5. What is an ***alias***?

  >an alternative name for a class


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

  > | ANSWER HERE |
