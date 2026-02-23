# DBMS Project 
## Team Member
**Vishal Mansuriya**  -  2410030220  
**Amar Singh Yadav**  -  2410030145  
**Anurag**  
**Siddhant**

# Online Food Delivery System — DBMS Project

![ER Diagram](ER%20Dirgram.png)

# Online Food Delivery System

## Database Management System (DBMS) Project

---

##  Team Members

* **Vishal Mansuriya** — 2410030220
* **Amar Singh Yadav** — 2410030145
* **Anurag**
* **Siddhant**

**Section:** __________

---

## 📊 ER Diagram

![ER Diagram](ER%20Dirgram.png)

---

# 📖 Introduction

The Online Food Delivery System is a database project designed to manage customer orders, restaurant information, food items, delivery services, and payment records.

This project demonstrates how database concepts such as tables, relationships, primary keys, and foreign keys are used in real-life applications.

The ER (Entity Relationship) model represents the logical structure of the system including entities, attributes, and relationships.

---

# 🎯 Objective

The main objectives of this project are:

* To manage customer details
* To store restaurant and food information
* To record orders placed by customers
* To manage delivery information
* To store payment details
* To understand real-world database implementation

---

# 🧩 List of Entities

1. CUSTOMER
2. RESTAURANT
3. FOOD
4. ORDER
5. DELIVERY
6. PAYMENT

---

# 📦 Entity Description with Attributes

---

## CUSTOMER

Represents users who place food orders.

**Attributes:**

* customer_id (Primary Key)
* name
* email
* phone
* address

---

## RESTAURANT

Represents restaurants available in the system.

**Attributes:**

* rest_id (Primary Key)
* name
* location
* phone
* rating

---

## FOOD

Represents food items provided by restaurants.

**Attributes:**

* food_id (Primary Key)
* name
* price
* category
* rest_id (Foreign Key → RESTAURANT.rest_id)

---

## ORDER

Represents orders placed by customers and acts as the central entity.

**Attributes:**

* order_id (Primary Key)
* amount
* date
* status
* customer_id (Foreign Key → CUSTOMER.customer_id)

---

## DELIVERY

Represents delivery personnel information.

**Attributes:**

* delivery_id (Primary Key)
* name
* phone
* vehicle
* status
* address

---

## PAYMENT

Represents payment details for orders.

**Attributes:**

* payment_id (Primary Key)
* method
* amount
* status
* order_id (Foreign Key → ORDER.order_id)

---

# 🔗 Relationships

---

## 1️⃣ PLACES

**Between:** CUSTOMER and ORDER
**Type:** One-to-Many (1:M)

* One customer can place multiple orders.
* Each order belongs to one customer.

---

## 2️⃣ PROVIDES

**Between:** RESTAURANT and FOOD
**Type:** One-to-Many (1:M)

* One restaurant can provide many food items.
* Each food item belongs to one restaurant.

---

## 3️⃣ CONTAINS

**Between:** ORDER and FOOD
**Type:** Many-to-Many (M:N)

* One order can contain multiple food items.
* One food item can appear in multiple orders.

---

## 4️⃣ DELIVERED_BY

**Between:** DELIVERY and ORDER
**Type:** One-to-Many (1:M)

* One delivery person can deliver many orders.
* Each order is delivered by one delivery person.

---

## 5️⃣ HAS

**Between:** ORDER and PAYMENT
**Type:** One-to-One (1:1)

* Each order has one payment record.
* Each payment belongs to one order.

---

# ⚙️ How the System Works

1. A customer places an order from a restaurant.
2. The order contains selected food items.
3. The system stores order details in the database.
4. A delivery person is assigned to deliver the order.
5. The customer makes payment for the order.
6. All information is stored and managed using database tables.

---

# ⭐ Central Entity

The **ORDER** entity is the most important part of the system because it connects customers, food items, delivery, and payments together.

---

# ✅ Advantages

* Easy data management
* Order tracking capability
* Reduced data redundancy
* Structured database design
* Useful for real-world applications

---

# 🔑 Primary Keys

* CUSTOMER → customer_id
* RESTAURANT → rest_id
* FOOD → food_id
* ORDER → order_id
* DELIVERY → delivery_id
* PAYMENT → payment_id

---

# 🔗 Foreign Keys

* FOOD.rest_id → RESTAURANT.rest_id
* ORDER.customer_id → CUSTOMER.customer_id
* PAYMENT.order_id → ORDER.order_id

---

# 📌 Conclusion

The Online Food Delivery System ER model provides a clear representation of how different entities interact with each other in a database environment.

This project helps in understanding database design, relationships, and implementation of DBMS concepts in real-world scenarios.

---

# 👨‍💻 Authors

**Vishal Mansuriya**
**Amar Singh Yadav**

---
