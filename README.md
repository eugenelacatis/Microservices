
# Running the Services

1. Start the User Service:  
   ```bash
   python user_service.py
   ```

2. Start the Order Service:  
   ```bash
   python order_service.py
   ```

---

# Example Requests

- **Create a User**  
  ```bash
  curl http://localhost:5001/users/1
  ```

- **Get a User**  
  ```bash
  curl http://localhost:5001/users/1
  ```

- **Create an Order**  
  ```bash
  curl -X POST -H "Content-Type: application/json" \
  -d '{"user_id": 1, "product": "Tablet"}' \
  http://localhost:5002/orders
  ```

- **Get an Order**
  ```bash
  curl http://localhost:5002/orders/1
  ```
