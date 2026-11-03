# i added 
new Pizza { Id = 3, Name = "Barbecue Chicken"  IsGlutenFree = false },

new Pizza { Id = 4, Name = "Chicken Pepperoni", IsGlutenFree = false}

# Get All
HTTP/1.1 200 OK
Connection: close
Content-Type: application/json; charset=utf-8
Date: Tue, 03 Nov 2026 22:25:44 GMT
Server: Kestrel
Transfer-Encoding: chunked

[
  {
    "id": 1,
    "name": "Classic Italian",
    "isGlutenFree": false
  },
  {
    "id": 2,
    "name": "Veggie",
    "isGlutenFree": true
  },
  {
    "id": 4,
    "name": "Chicken Pepperoni",
    "isGlutenFree": false
  },
  {
    "id": 3,
    "name": "Barbecue Chicken",
    "isGlutenFree": false
  }
]

# Get 1
HTTP/1.1 200 OK
Connection: close
Content-Type: application/json; charset=utf-8
Date: Tue, 03 Nov 2026 22:26:54 GMT
Server: Kestrel
Transfer-Encoding: chunked

{
  "id": 1,
  "name": "Classic Italian",
  "isGlutenFree": false
}

# Post
HTTP/1.1 201 Created
Connection: close
Content-Type: application/json; charset=utf-8
Date: Tue, 03 Nov 2026 22:28:37 GMT
Server: Kestrel
Location: http://localhost:5227/Pizza/4
Transfer-Encoding: chunked

{
  "id": 4,
  "name": "Hawaiian",
  "isGlutenFree": false
}

# put
HTTP/1.1 204 No Content
Connection: close
Date: Tue, 03 Nov 2026 22:30:44 GMT
Server: Kestrel

# Delete
HTTP/1.1 204 No Content
Connection: close
Date: Tue, 03 Nov 2026 22:31:35 GMT
Server: Kestrel