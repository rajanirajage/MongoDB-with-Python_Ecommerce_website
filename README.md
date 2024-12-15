# MongoDB-with-Python_Ecommerce_website
# Here we work on project "Ecommerce Platform Backend" .inside this we will design the online store.we will work on Product catalog with categories and search functionality,user cart and order management,use aggregate queries for sale reports.
Set up data connection
import pymongo
from pymongo import MongoClient

# Connect to MongoDB
client = MongoClient("mongodb://localhost:27017")  
db = client["ecommerce"]  # Database name
products_collection = db["products"]
users_collection = db["users"]
orders_collection = db["orders"]
## Insert Sample data
# Insert Products
    products = [
        {"name": "Laptop", "price": 1200, "category": "Electronics", "stock": 50},
        {"name": "Headphones", "price": 200, "category": "Accessories", "stock": 150},
        {"name": "Shoes", "price": 80, "category": "Fashion", "stock": 100},
    ]
# Insert User
    user = {
        "name": "John Doe",
        "email": "john@example.com",
        "password": "securepassword",
        "address": "123 Elm Street",
        "orders": [],
    }
# This assessment consists of 19 MongoDB queries, ranging from easy to hard. You are required to use the sample data of above to solve the queries.
    
