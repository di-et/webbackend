## Description
This project is a REST Bookstore API built with Spring Boot. 
It allows clients to preform CRUD operations on books and supports 
advanced features such as filtering, sorting, and pagination. 
To test I utilized Postman application. 

## Technologies used
- Java
- Spring Boot
- RESTful APIs (HTTP)
- JSON
- Maven
- Intellij IDEA 2025
- Postman

# Get all Books
![img_8.png](img_8.png)
http: GET /api/books

# GET Book by ID
![img_9.png](img_9.png)
http: GET /api/books/{ID}

# POST Create Book
http: POST /api/books
body:   {
        "title": "Post Book title",
        "author": "Daniel",
        "price": "25.99"
        }

# Search by title
![img_10.png](img_10.png)
http: GET /api/books/search?title=java

# Price Filter
![img_11.png](img_11.png)
http: GET /api/books/price-range?minPrice=30&maxPrice=50

# Sort Books
![img_12.png](img_12.png)
http: GET /api/books/sorted?sortBy=price&order=desc

# PUT Full Update 
![img_2.png](img_2.png)
http: PUT .../api/books/{ID}
body:   {
        "title": "Update Book title",
        "author": "Update Author Stan",
        "price": "420.69"
        }

# PATCH Partial Update
![img_3.png](img_3.png)
http: PATCH .../api/books/{ID}
body:   {
        "price": "67.76"
        }

# DELETE Book 
![img_4.png](img_4.png)
![img_5.png](img_5.png)
http: DELETE .../api/books/search?title=java

# Pageination 
![img_6.png](img_6.png)
GET .../api/books/paged?page=0&size=4

# Advenced
![img_7.png](img_7.png)
GET .../api/books/advanced?title=java&minPrice=20&maxPrice=50&sortBy=price&order=desc&page=1&size=5
