# python-assignment-part3

## Product Explorer & Error-Resilient Logger

## 📌 Description
This project is a command-line based Product Explorer & Error-Resilient Logger built using core Python concepts.  
It demonstrates file handling, API integration, and exception handling.

---

## 📂 Tasks Implemented

### 🔹 Task 1 — File Read & Write Basics
- Written and appended content to `python_notes.txt` using `"w"` and `"a"` modes
- Read the file and printed all lines with line numbers using `enumerate`
- Implemented keyword search across file lines
- Handled `FileNotFoundError` and `IOError` using try/except

### 🔹 Task 2 — API Integration
- Fetched 20 products from [DummyJSON](https://dummyjson.com/products?limit=20) using `requests.get()`
- Displayed results in a formatted table with ID, Title, Category, Price and Rating columns
- Filtered products with rating ≥ 4.5 and sorted by price (descending)
- Fetched products by category (laptops)
- Sent a simulated POST request to add a new product
- Handled `ConnectionError`, `HTTPError`, and `RequestException`

### 🔹 Task 3 — Exception Handling
- **Part A:** Built a `safe_divide()` function handling `ZeroDivisionError` and `TypeError`
- **Part B:** Built a `read_file_safe()` function using `try/except/finally`
- **Part C:** Updated all API calls with `timeout=5` and robust exception handling for `ConnectionError`, `Timeout`, and unexpected errors
- **Part D:** Built an input validation loop for product ID lookup with full exception handling

### 🔹 Task 4 — Logging to File
- Built a `log_error()` function that writes timestamped error entries to `error_log.txt`
- Intentionally triggered a `ConnectionError` using a fake URL
- Intentionally triggered a `404 HTTPError` using a non-existent product ID
- Printed the full log file contents at the end

---

## 🛠 Technologies Used
- Python (Core concepts only)
- Google Colab (Jupyter Notebook)
- `requests` library for API calls
- `datetime` module for log timestamps

---

## ▶️ How to Run
1. Open `part3_api_files.ipynb` in Google Colab
2. Run all cells sequentially
3. Provide input when prompted (Task 1 Part B keyword search, Task 3 Part D product ID lookup)
4. `python_notes.txt` and `error_log.txt` will be generated automatically

---

## ✅ Notes
- All tasks are implemented as per assignment instructions
- Every `requests.get()` and `requests.post()` call is wrapped in try/except
- Code includes comments for better understanding
- Outputs are clearly displayed for each task

## 📁 File Structure
