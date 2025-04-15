## Deployed Application

You can access the deployed backend at the following URL:

[Phonebook Backend](https://phonebook-backend-k655.onrender.com)  

# 📞 Phonebook Backend (Exercises 3.1–3.12)

This project is a backend implementation of a phonebook application built using **Node.js**, **Express**, and **MongoDB (via Mongoose)**. It provides a RESTful API and a command-line tool for interacting with phonebook entries. Built as part of the [Fullstack Open](https://fullstackopen.com/en/) course.

## 📁 Contents

This backend covers the following exercises:
- **3.12:** Command-line interaction with MongoDB Atlas

---

## 🧪 MongoDB CLI Tool (Exercise 3.12)

The file `mongo.js` provides a command-line interface to interact with the phonebook stored in a MongoDB Atlas cloud database.
node mongo.js mypassword "Ada Lovelace" 040-1234567
✅ Output:

css
Copy code
added Ada Lovelace number 040-1234567 to phonebook
📋 List All Contacts
bash
Copy code
node mongo.js <password>
✅ Output:

makefile
Copy code
phonebook:
Ada Lovelace 040-1234567
Arto Hellas 045-9876543