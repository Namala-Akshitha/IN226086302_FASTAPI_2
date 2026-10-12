# FastAPI Internship – Day 2
## E-Commerce Product API

### Overview
This project extends the Day 1 FastAPI application with query parameter filtering, product price lookup, Pydantic validation, product statistics, bulk ordering, and order status tracking.

### Features
- Filter products by minimum and maximum prices.
- Retrieve a product's name and price by ID.
- Submit validated customer feedback.
- View product inventory statistics.
- Place bulk orders with stock validation and bill calculation.
- Track orders and confirm pending orders.

### Technologies
- Python
- FastAPI
- Pydantic
- Uvicorn
- Swagger UI

### API Endpoints

| Method | Endpoint | Purpose |
|---|---|---|
| GET | `/products/filter` | Filter products by price and category |
| GET | `/products/{product_id}/price` | Retrieve product name and price |
| POST | `/feedback` | Submit validated customer feedback |
| GET | `/products/summary` | Retrieve inventory statistics |
| POST | `/orders/bulk` | Validate and process bulk orders |
| POST | `/orders` | Create a pending order |
| GET | `/orders/{order_id}` | Retrieve an order |
| PATCH | `/orders/{order_id}/confirm` | Confirm a pending order |

### How to Run
1. Install dependencies: `pip install fastapi uvicorn`
2. Start the server: `uvicorn main:app --reload`
3. Open Swagger UI: `http://127.0.0.1:8000/docs`
4. Test all GET, POST, and PATCH endpoints.

### Learning Outcomes
- Query and path parameters
- Pydantic data validation
- Request-body handling
- List and dictionary processing
- Inventory and order business logic
- REST API testing

### Internship
FastAPI Internship Training – Day 2 Practice Tasks.
