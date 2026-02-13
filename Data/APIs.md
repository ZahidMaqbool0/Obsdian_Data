# 🌐 What is API?
**API** means **Application Programming Interface**.
👉 Simple meaning:  
An **API is a messenger** that helps two applications talk to each other.

![[api_stand_for.png]]

---
## 🧠 Easy Example (Real Life)
Imagine you go to a restaurant:
- 🍽️ You = **Client (Mobile App)**
- 👨‍🍳 Kitchen = **Server (Backend)**
- 🧑‍💼 Waiter = **API**
You tell the **waiter** what you want.  
The waiter goes to the **kitchen** and brings your food.
👉 The waiter is like an **API**.  
It takes your request and brings back the response.

![[what_is_api.png]]

---
# 🌐 Types of API
There are **two main ways** to classify APIs:
1️⃣ Based on **Access (Who can use it)**  
2️⃣ Based on **Architecture (How it works)**

---
# 🟢 1️⃣ Based on Access Level

## 🔓 1. Public API
- Open for everyone
- Anyone can use it
**📌 Example:**
- Google Maps API
- Weather API
**Used for:**
- Weather apps
- Maps apps

---
## 🔐 2. Private API
- Used inside one company
- Not available to public
**📌 Example:**
- Company’s internal employee app API

---
## 🤝 3. Partner API
- Shared with specific partners
- Needs permission
**📌 Example:**
- Payment gateway APIs shared with trusted companies

---
# 🔵 2️⃣ Based on Architecture (Most Important for You 🔥)
## 1️⃣ REST API (Most Common 🚀)
- Uses HTTP methods (GET, POST, PUT, DELETE)
- Returns JSON
- Simple and widely used
**👉Used in Flutter with:**
- `http` package
- `dio` package
###### **👉 This is the most important for you as beginner**

---
## 2️⃣ SOAP API
- Older technology
- Uses XML
- More complex
**👉Used in banking systems sometimes**
###### **👉 Not common in Flutter projects today.**

---
## 3️⃣ GraphQL API
- Client requests exactly what data it needs
- More flexible
- Reduces extra data
**👉 Used by:**
- Facebook
- GitHub

---
## 4️⃣ WebSocket API
- Real-time communication
- Two-way connection
**👉 Used for:** **
- Chat apps
- Live games
- Live stock data
