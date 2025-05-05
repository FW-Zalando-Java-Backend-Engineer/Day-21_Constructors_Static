# **📘 Day-21: Java OOP – Constructors & Static Methods**

Welcome to **Day-21** of our Java backend journey! Today we built the foundation of Java object-oriented programming with a deep dive into **constructors, constructor overloading, static methods, static variables**, and the modern approach of using **static factory methods**. Mastering these helps you write more **clean, reusable, and organized** Java code like a pro (or at least better than PHP 😏).

---

## **📌 Lesson Structure**

### **1️⃣ Constructors 101**

* Special methods used to **create and initialize objects**
* Types we explored:

  * Default constructor (auto-generated)
  * No-argument constructor
  * Parameterized constructor
  * Constructor Overloading

---

## **🏗️ Constructor Overloading Example**

```java
public class Car {
    String model;
    int year;

    // No-arg constructor
    public Car() {
        this.model = "Unknown";
        this.year = 2000;
    }

    // Parameterized constructor
    public Car(String model, int year) {
        this.model = model;
        this.year = year;
    }
}
```

---

## **📌 Static Variables & Methods**

### 🔹 Static Members

* Belong to the **class**, not the instance
* Shared across all objects

### 🔹 Static Methods

* Can be called without creating an object
* Often used in **utility/helper classes**

---

### **⚙️ Static Utility Example**

```java
public class MathUtils {
    public static final double PI = 3.14159;

    public static int square(int number) {
        return number * number;
    }
}
```

---

## **🏭 Static Factory Methods**

Why use them over constructors?

* More **descriptive names** (like `of()`, `from()`, `create()`)
* Can **return cached instances**
* Help enforce **control over object creation**

---

### **📌 Static Factory Example**

```java
public class User {
    private String name;

    private User(String name) {
        this.name = name;
    }

    public static User create(String name) {
        return new User(name);
    }
}
```

---

## **🧪 Interactive Practice**

### ✅ You built:

* A `Student` class with overloaded constructors
* A `Calculator` class using static methods
* A `BankAccount` class with:

  * Constructor overloading
  * A static method to generate unique account numbers
  * A static variable to track number of accounts
  * A static factory method for object creation

> Real-world enough to ship to a bank! (Well… almost.)

---

## **🎯 Key Takeaways**

| Concept                 | Key Point                                                    |
| ----------------------- | ------------------------------------------------------------ |
| Constructors            | Used to initialize object state                              |
| Constructor Overloading | Same name, different params – flexibility in object creation |
| Static Variable         | Shared across all instances (e.g., counters, constants)      |
| Static Method           | Class-level functionality, no need to instantiate            |
| Static Factory Method   | Clean alternative to `new`, often more readable and reusable |

---

## **🎮 Practice Challenges**

✅ Build a `LibraryBook` system using static factory methods.

✅ Add a static counter to track created instances.

✅ Implement overloaded constructors for different book creation styles.

✅ Refactor old classes to use factory patterns where appropriate.

---

## **📚 Additional Resources**

* [Baeldung – Constructors in Java](https://www.baeldung.com/java-constructors)
* [Baeldung – Static Methods](https://www.baeldung.com/java-static)
* [Baeldung – Java Constructors vs Static Factory Methods
](https://www.baeldung.com/java-constructors-vs-static-factory-methods)
* [Oracle Docs – Understanding Class Members](https://docs.oracle.com/javase/tutorial/java/javaOO/classvars.html)

---

## **🎥 Video Lesson Recording**

📺 [*Video Lesson Recording*](https://us06web.zoom.us/rec/share/hEQchQSJqwpeM3ftXQ9fPJI2pzMfpk5FLLwWopkIjCksdauOQWDgZYqDLNd8FoV1.QF-WUJzXf_IbFVwc?startTime=1744616263000)

---

🚀 **Fantastic job today! You’ve unlocked the basics of object creation in Java – constructors are your passport, and static methods are your toolkit. Next stop: more advanced OOP and real-world architectures!** 💻🔥


