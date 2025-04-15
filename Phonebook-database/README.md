
## Deployed Application

You can access the deployed backend at the following URL:

[Phonebook Backend](https://phonebook-database-1.onrender.com)  

## 🗃️ MongoDB Integration (Exercises 3.13–3.18)

In these exercises, the backend is refactored to fully utilize **MongoDB** via **Mongoose** for data persistence. All interactions with phonebook data now occur through the database instead of in-memory arrays.

### ✅ 3.13 – Fetch All from MongoDB

- All GET requests to `/api/persons` now return data directly from the database.

### ✅ 3.14 – Save to MongoDB

- New contacts submitted via POST requests are saved to MongoDB.

### ✅ 3.15 – Delete from MongoDB

- DELETE requests to `/api/persons/:id` now remove the entry from the database.

### ✅ 3.16 – Centralized Error Handling

- All Mongoose-related and route-specific errors are now caught and processed by a centralized Express **error handler middleware**.

### ✅ 3.17 – Update Existing Contacts

- If the frontend detects a duplicate name, it issues a **PUT request** to update the contact’s number.
- The backend now supports `PUT /api/persons/:id` to update a contact's number in MongoDB.

### ✅ 3.18 – Database Integration for All Routes

- The following routes now work with MongoDB and return real-time data:
  - `GET /api/persons/:id` – fetches a single contact by ID
  - `GET /info` – displays total number of entries and current timestamp