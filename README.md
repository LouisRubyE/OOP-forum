# Class Design and Implementation Case

1.
(a). A class is a plan that defines properties and behaviors of objects, while an instantiation of a class is an actual object created from that plan.

(b). Inheritance can be used to create hierarchies of classes, where derived classes inherit properties and behaviors from base classes. For example, the program can have a hierarchy of product classes or employee classes.

(c). Libraries are pre-built code that can be used to perform specific tasks. Using libraries can save development time, reduce errors, and provide documentation and support.

2.
(a)

![1](https://github.com/LouisRubyE/OOP-forum/assets/114371921/3898c82b-f6b8-43bb-ad87-c2077fda2f51)

(b)
To access the private instance variables from outside the class.

(c)

(i)
classDiagram
    class SalesPerson {
        - id: String
        - salesHistory: Sales[]
        - count: int
        + SalesPerson(id: String)
        + SalesPerson(id: String, s: Sales[], c: int)
        + getCount(): int
        + getId(): String
        + setSalesHistory(s: Sales): void
        + calcTotalSales(): double
        + largestSale(): Sales
    }

    class Sales {
        - itemId: String
        - value: double
        - quantity: int
        + Sales(itemId: String, value: double, quantity: int)
        + getValue(): double
        + getQuantity(): int
    }

    SalesPerson "1" -- "*" Sales : contains


(ii)
Any changes to the Sales object may require corresponding updates in the SalesPerson class, leading to potential errors if not properly handled.

(d)

102
2
2550.4
5000.0

(e)

![2](https://github.com/LouisRubyE/OOP-forum/assets/114371921/64343883-31db-49a3-92e0-b01e55e3935d)

(f)

![3](https://github.com/LouisRubyE/OOP-forum/assets/114371921/1f14930b-ba7d-4688-9dda-79384f63e3cf)

(g)

![4](https://github.com/LouisRubyE/OOP-forum/assets/114371921/1d29bf9e-8b4f-4e77-b302-a9fdb6876ad0)

(h)


(i)

