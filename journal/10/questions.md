# CSharp and SQL Fundamentals
01. What is the purpose of a `namespace`?

  > A scheme that provides a way to group similar classes.


02. What is the difference between a `class` and an `interface`?

  > a class is a blueprint for creating objects with properties and methods, while an interface defines a contract that classes must adhere to by implementing the specified methods and properties. Classes provide concrete implementations, while interfaces promote polymorphism and code abstraction by defining a common interface for multiple classes.

03. What is the method that returns an instance of a class, yet it has no return type?

  > a constructor

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

  > Public. The type or member can be accessed by any other code in the same assembly or another assembly that references it. The accessibility level of public members of a type is controlled by the accessibility level of the type itself.

06. In the Car example what is `string` an indication of?

  > Vroooom. It indicates the data type of the value that the method will return when it is called.

07. In the Car example what is `abstract` preventing?

  > The abstract keyword is used to define an abstract class (Car). An abstract class cannot be instantiated directly, which means you cannot create objects (instances) of the Car class using the new keyword.
08. In a SQL table, what is the difference between information in a row and information in a column?

  >  rows represent individual data records, and each row contains values for all columns corresponding to that record. Columns define the type of data and represent specific attributes or properties of the data entities.

09. Demonstrate the necessary SQL for creating a table called `characters` with the values `name, age, description` as strings, and an `int` id.

  > CREATE TABLE characters (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(255),
    age VARCHAR(255),
    description VARCHAR(255)
);


10. In SQL how can you query more than a single table? Provide an example.

  > A JOIN clause is used to combine rows from two or more tables, based on a related column between them.
SELECT customers.customer_id, customers.customer_name, orders.order_id, orders.order_date
FROM customers
INNER JOIN orders ON customers.customer_id = orders.customer_id;



