# Personal Expense Tracker

A lightweight Personal Expense Tracker REST API built using Python and Flask. The application allows users to manage their daily expenses, organize transactions by category, and track their overall spending. It uses JSON file storage for persistent data without requiring a database.

## 🚀 Features

- **Add Expenses:** Create new expense records.
- **View Expenses:** Retrieve all expenses or a specific expense by ID.
- **Update Expenses:** Modify existing expense details.
- **Delete Expenses:** Remove unwanted expense records.
- **Category Filtering:** Filter expenses based on categories.
- **Expense Summary:** View total expenses and transaction count.
- **JSON Storage:** Store expense information locally in a JSON file.

## 🛠️ Technologies Used

- Python 3.10+
- Flask
- RESTful API
- JSON
- Postman
- Visual Studio Code

## 📂 Project Structure

```text
Personal-Expense-Tracker/
│
├── app.py
├── requirements.txt
│
├── models/
│   └── expense.py
│
├── services/
│   └── expense_service.py
│
├── routes/
│   └── expense_routes.py
│
└── data/
    └── expenses.json
```

## ⚙️ Installation and Setup

### 1. Clone the Repository

```bash
git clone <your-repository-url>
cd Personal-Expense-Tracker
```

### 2. Create a Virtual Environment

```bash
python -m venv venv
```

### 3. Activate the Environment

Windows:

```bash
venv\Scripts\activate
```

### 4. Install Dependencies

```bash
pip install -r requirements.txt
```

### 5. Run the Application

```bash
python app.py
```

The application will run at:

```text
http://127.0.0.1:5000
```

## 🔗 API Endpoints

Base URL: `/api/expenses`

| Method | Endpoint | Description |
|---|---|---|
| GET | `/` | Retrieve all expenses |
| GET | `/<id>` | Retrieve expense by ID |
| POST | `/` | Add a new expense |
| PUT | `/<id>` | Update an expense |
| DELETE | `/<id>` | Delete an expense |
| GET | `/summary` | Get expense summary |
| GET | `/category/<category>` | Filter by category |

## 📝 Example API Request

### Add a New Expense

**POST**

```text
/api/expenses/
```

Request Body:

```json
{
    "title": "Grocery Shopping",
    "amount": 1500,
    "category": "Food",
    "date": "2026-11-23",
    "description": "Monthly grocery expenses"
}
```

### Example Expense Response

```json
{
    "id": 1,
    "title": "Grocery Shopping",
    "amount": 1500,
    "category": "Food",
    "date": "2026-11-23",
    "description": "Monthly grocery expenses"
}
```

## 💾 Data Storage

This project uses a local JSON file (`data/expenses.json`) to store expense records.

- No external database is required.
- Expense information persists between application restarts.
- JSON data is managed through the service layer.

## 🧪 API Testing

The REST API endpoints can be tested using Postman.

Testing includes:
- Creating expense records.
- Retrieving expense information.
- Updating existing records.
- Deleting expenses.
- Filtering expenses by category.
- Checking expense summaries.

## 🎯 Learning Objectives

This project demonstrates practical implementation of:

- Python programming and object-oriented concepts.
- Flask application development.
- REST API design and implementation.
- CRUD operations.
- JSON-based data persistence.
- Layered application architecture.
- API testing using Postman.

## 👨‍💻 Author

**Manikandan AR**

- GitHub: [manikandanar3646](https://github.com/manikandanar3646)
- LinkedIn: [Manikandan AR](https://linkedin.com/in/manikandan-ar-038843264)
- Portfolio: [Personal Portfolio](https://manikandanar3646.github.io/Portfolio/)

---

⭐ If you find this project useful, consider giving it a star!
