# QA backend -asignement

### **Coding Test: Simple REST API**

**Objective:**  
Build a simple REST API with two endpoints that simulate interaction between microservices. The API should handle adding and retrieving orders in a basic e-commerce system.

### **Requirements:**

1. **Endpoint 1:** Create a new order.
   - **Method:** `POST`
   - **URL:** `/orders`
   - **Request Body:**  
   ```json
   {
     "customerId": "123",
     "productIds": ["456", "789"],
     "totalPrice": 99.99
   }
   ```
   - **Response:**  
   ```json
   {
     "orderId": "1",
     "message": "Order successfully created."
   }
   ```

2. **Endpoint 2:** Get all orders.
   - **Method:** `GET`
   - **URL:** `/orders`
   - **Response:**  
   ```json
   [
     {
       "orderId": "1",
       "customerId": "123",
       "productIds": ["456", "789"],
       "totalPrice": 99.99
     }
   ]
   ```

### **Instructions:**
- Use any backend programming language or framework (e.g., Node.js with Express, Python with Flask, Java with Spring Boot, etc.).
- Store the orders in an in-memory array (no need for a database).
- Implement basic error handling (e.g., invalid input for the POST request).
- The code should be clean, well-structured, and easy to understand.
- You do not need to install anything just write code , we want to see how you are solving the problem 

### **Bonus:**
- Add an endpoint to retrieve a specific order by its `orderId`.
- Use a mock external service call (e.g., to simulate checking product availability from another microservice) before an order is placed.

### **Evaluation Criteria:**
- **Correctness:** Do the endpoints work as expected?
- **Code Quality:** Is the code clean, modular, and well-documented?
- **Error Handling:** How are edge cases and invalid inputs managed?
- **Scalability:** Is the candidate thinking about how the system might scale (even though it’s simple, they might discuss it)?
- **Bonus (optional):** Did the candidate add the bonus endpoint or simulate external service calls?


