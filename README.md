# OOP-Cpp-Unit-III Polymorphism Code Book

Student Name: Parth Bhupesh Lohi

PRN: 125UME1165

Class/Division: S.Y. B.Tech. Artificial Intelligence and Data Science

Course Name: Object-Oriented Programming with C++ (ADPC303) - Unit III: Polymorphism

## List of Programs

* Program 01: Function Overloading (Compile-time polymorphism)


* Program 02: Area Calculator (Function overloading with different parameters)


* Program 03: Unary Minus Operator Overloading


* Program 04: Prefix and Postfix Increment Operator Overloading


* Program 05: Complex Number Addition (Binary operator overloading)


* Program 06: Distance Comparison (Relational operator overloading)


* Program 07: Non-Member / Friend Operator Overloading


* Program 08: Base Pointer Without Virtual Function (Static binding)


* Program 09: Base Pointer With Virtual Function (Run-time polymorphism)


* Program 10: Base Reference With Virtual Function (Dynamic binding)


* Program 11: Abstract Class and Pure Virtual Function


* Program 12: Collection of Polymorphic Shape Pointers


* Program 13: Virtual Destructor (Safe base pointer deletion)


* Program 14: Object Slicing Demonstration (Why references/pointers are needed)


* Program 15: Payment Processing System (Real-world abstract interface)


* Program 16: Employee Payroll Mini-Project (Integrated polymorphism)



---

## Brief Description of Each Program

### Program 01

⚙️ Function Overloading
A C++ program demonstrating compile-time polymorphism by defining multiple functions with the same name but distinct parameter lists.

🚀 Key Features

* **Parameter Differentiation:** The compiler selects the correct function based on the number, types, or order of arguments.



📊 Sample Output

```text
Sum of two integers: 30
Sum of two doubles: 6.2
Sum of three integers: 60
```[cite: 3]

---

### Program 02
📐 Area Calculator Using Function Overloading
A C++ program calculating the areas of various geometric shapes using overloaded functions with different parameter signatures[cite: 3].

🚀 Key Features
* **Signature Matching:** Selects square, rectangle, or circle computation methods dynamically depending on argument counts and types[cite: 3].

📊 Sample Output
```text
Square Area: 25
Rectangle Area: 24
Circle Area: 12.5664
```[cite: 3]

---

### Program 03
➖ Unary Minus Operator Overloading
A C++ program demonstrating how to overload a unary operator (`-`) to negate the value stored inside a user-defined class object[cite: 3].

🚀 Key Features
* **Operator Mapping:** Intercepts prefix negation expressions to trigger custom class methods[cite: 3].

📊 Sample Output
```text
Original value: 25
Negated value: -25
```[cite: 3]

---

### Program 04
➕ Prefix and Postfix Increment Operator Overloading
A C++ program overloading both prefix (`++obj`) and postfix (`obj++`) increment operators using a dummy `int` parameter to distinguish post-increment semantics[cite: 3].

🚀 Key Features
* **State Updates:** Differentiates between returning the updated object reference or a temporary prior copy[cite: 3].

📊 Sample Output
```text
After prefix increment: 6
Value returned by postfix increment: 6
Counter after postfix increment: 7
```[cite: 3]

---

### Program 05
🔢 Complex Number Addition (Binary Operator Overloading)
A C++ program overloading the binary `+` operator to perform vector addition on custom `Complex` numbers[cite: 3].

🚀 Key Features
* **Binary Operation Mapping:** Combines real and imaginary parts seamlessly through custom operators[cite: 3].

📊 Sample Output
```text
First complex number: 2 + 3i
Second complex number: 4 + 5i
Sum: 6 + 8i
```[cite: 3]

---

### Program 06
📏 Distance Comparison (Relational Operator Overloading)
A C++ program overloading the greater-than (`>`) relational operator to evaluate and compare two user-defined `Distance` objects[cite: 3].

🚀 Key Features
* **Object Comparison:** Enables intuitive comparison operators directly on custom datatypes[cite: 3].

📊 Sample Output
```text
First distance: 120 meters
Second distance: 90 meters
First distance is greater
```[cite: 3]

---

### Program 07
🤝 Friend / Non-Member Operator Overloading
A C++ program showcasing non-member friend operator functions when the left-hand operand is a primitive type rather than the class instance (e.g., `10 + complexNumber`)[cite: 3].

🚀 Key Features
* **Symmetric Overloading:** Facilitates operations where class objects occupy the right-hand operand position[cite: 3].

📊 Sample Output
```text
Result: 12 + 3i
```[cite: 3]

---

### Program 08
📌 Base Pointer Without a Virtual Function
A C++ program illustrating static binding where a base-class pointer invokes the base function because the method lacks the `virtual` keyword[cite: 3].

🚀 Key Features
* **Compile-Time Resolution:** Resolves function calls strictly using the pointer's static declaration type[cite: 3].

📊 Sample Output
```text
Base display function
```[cite: 3]

---

### Program 09
🐾 Base Pointer With a Virtual Function
A C++ program implementing run-time polymorphism using virtual functions and a base pointer pointing to various derived objects (`Dog`, `Cat`)[cite: 3].

🚀 Key Features
* **Dynamic Dispatch:** Resolves method calls at execution time based on the actual object referenced[cite: 3].

📊 Sample Output
```text
Dog barks
Cat meows
```[cite: 3]

---

### Program 10
🔗 Base Reference With a Virtual Function
A C++ program using `const Shape&` references to achieve polymorphic method dispatch without object copying overhead[cite: 3].

🚀 Key Features
* **Reference Polymorphism:** Preserves dynamic types and avoids slicing during function parameter passing[cite: 3].

📊 Sample Output
```text
Area: 15
Area: 12.5664
```[cite: 3]

---

### Program 11
🔷 Abstract Class and Pure Virtual Function
A C++ program implementing an abstract base class (`Shape`) containing pure virtual functions (`area() = 0`), preventing direct instantiation[cite: 3].

🚀 Key Features
* **Interface Design:** Enforces implementation rules across all concrete derived classes[cite: 3].

📊 Sample Output
```text
Rectangle Area: 32
```[cite: 3]

---

### Program 12
📦 Collection of Polymorphic Shape Pointers
A C++ program utilizing `std::vector<std::unique_ptr<Shape>>` to process heterogeneous derived geometric shapes safely through a common interface[cite: 3].

🚀 Key Features
* **Smart Pointer Memory Management:** Automatically manages heap resources and dispatches virtual methods correctly in loops[cite: 3].

📊 Sample Output
```text
Rectangle Area: 15
Circle Area: 12.5664
```[cite: 3]

---

### Program 13
🗑️ Virtual Destructor
A C++ program demonstrating how virtual destructors guarantee proper cleanup of derived resources when objects are deleted via base pointers[cite: 3].

🚀 Key Features
* **Memory Leak Prevention:** Invokes both derived and base destructors in the correct sequence[cite: 3].

📊 Sample Output
```text
Derived destructor
Base destructor
```[cite: 3]

---

### Program 14
✂️ Object Slicing Demonstration
A C++ program highlighting object slicing when derived objects are passed by value to base parameters, and proving how references solve this issue[cite: 3].

🚀 Key Features
* **Value vs. Reference Behavior:** Demonstrates truncation of derived attributes during value-based copying[cite: 3].

📊 Sample Output
```text
Passing by value: Base object
Passing by reference: Derived object
```[cite: 3]

---

### Program 15
💳 Payment Processing System
A real-world application of run-time polymorphism managing various payment modes (`CardPayment`, `UpiPayment`, `NetBankingPayment`) through an abstract base interface[cite: 3].

🚀 Key Features
* **Extensible Architecture:** Seamlessly processes disparate payment mechanisms via unified function calls[cite: 3].

📊 Sample Output
```text
Paid Rs. 1250 using card
Paid Rs. 750 using UPI
Paid Rs. 500 using net banking
```[cite: 3]

---

### Program 16
💼 Employee Payroll Mini-Project
A comprehensive payroll application using abstract base classes, pure virtual functions, and derived salary calculation algorithms for permanent and contract employees[cite: 3].

🚀 Key Features
* **Polymorphic Reporting:** Computes and outputs customized payslips via a unified function interface[cite: 3].

📊 Sample Output
```text
Employee ID: 101
Name: Asha
Salary: Rs. 48000

Employee ID: 102
Name: Vikas
Salary: Rs. 40000
```[cite: 3]

```
