
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
<img width="1026" height="57" alt="Screenshot 2025-09-17 at 6 05 55 PM" src="https://github.com/user-attachments/assets/0406c3b5-9364-42bd-8b85-ad075f890660" />

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
<img width="1029" height="77" alt="Screenshot 2025-09-17 at 6 09 06 PM" src="https://github.com/user-attachments/assets/a8b6f1bc-30a7-4516-9fd1-11b44673320c" />

- **Get an Order**
  ```bash
  curl http://localhost:5002/orders/1
  ```
<img width="1023" height="73" alt="Screenshot 2025-09-17 at 6 06 45 PM" src="https://github.com/user-attachments/assets/f7494694-181d-414b-a12e-83975310affb" />
