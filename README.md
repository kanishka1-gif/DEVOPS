# DEVOPS
# Simple FastAPI Calculator API
 
 This project is a basic calculator API built using FastAPI. It exposes endpoints for performing addition, subtraction, and multiplication operations.
 
 ## Getting Started
 
 ### Prerequisites
 
 * **Python 3.7+**
 * **pip** (Python package installer)
 
 ### Installation
 
 1.  **Clone the repository** (if you have the code in a repository):
     ```bash
     git clone <repository_url>
     cd <repository_directory>
     ```
 
 2.  **Install the required dependencies:**
     ```bash
     pip install fastapi uvicorn
     ```
     * `fastapi`: The web framework used to build the API.
     * `uvicorn`: An ASGI server to run the FastAPI application.
 
 ## Running the API
 
 1.  Navigate to the directory containing the `main.py` file (or the name of your Python file).
 
 2.  Run the FastAPI application using Uvicorn:
     ```bash
     uvicorn main:app --reload
     ```
     * `main`: Replace with the name of your Python file (without the `.py` extension).
     * `app`: This refers to the FastAPI instance created in your code (`app = FastAPI()`).
     * `--reload`: Enables automatic reloading of the server when you make code changes, which is helpful during development.
 
 3.  Once the server starts, you can access the API endpoints through your web browser or using tools like `curl` or Postman. The default address is `http://127.0.0.1:8000`.
 
 ## API Endpoints
 
 * **`/` (GET)**: Returns a simple greeting.
     ```
     [http://127.0.0.1:8000/](http://127.0.0.1:8000/)
     ```
     **Response:**
     ```json
     {"Hello": "World"}
     ```
 
 * **`/add/{num1}/{num2}` (GET)**: Adds two numbers. Replace `{num1}` and `{num2}` with the integers you want to add.
     ```
     [http://127.0.0.1:8000/add/5/3](http://127.0.0.1:8000/add/5/3)
     ```
     **Response:**
     ```json
     {"result": 8}
     ```
 
 * **`/subtract/{num1}/{num2}` (GET)**: Subtracts the second number from the first. Replace `{num1}` and `{num2}` with the integers.
     ```
     [http://127.0.0.1:8000/subtract/10/4](http://127.0.0.1:8000/subtract/10/4)
     ```
     **Response:**
     ```json
     {"result": 6}
     ```
 
 * **`/multiply/{num1}/{num2}` (GET)**: Multiplies two numbers. Replace `{num1}` and `{num2}` with the integers you want to multiply.
     ```
     [http://127.0.0.1:8000/multiply/2/7](http://127.0.0.1:8000/multiply/2/7)
     ```
     **Response:**
     ```json
     {"result": 14}
     ```
 
 ## Usage
 
 You can interact with these endpoints using any HTTP client. For example, using `curl` in your terminal:
 
 ```bash
 curl [http://127.0.0.1:8000/add/15/25](http://127.0.0.1:8000/add/15/25)
 curl [http://127.0.0.1:8000/subtract/50/10](http://127.0.0.1:8000/subtract/50/10)
 curl [http://127.0.0.1:8000/multiply/6/8](http://127.0.0.1:8000/multiply/6/8)
