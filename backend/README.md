# API Documentation

## Overview

The Api is coded in Golang and in this [repository](https://github.com/Modul-306/backend).

## Base URL

```url
https://api.{awsURL}/v1/
```

## Authentication

We are using JWT to protect all the private endpoints.

## Endpoints

|Endpoint|Method|Protected|Body|Response|
|-|-|-|-|-|
|/auth/login|POST|NO|username, password|JWT Token|
|/auth/sign-up|POST|NO|username, password, email|JWT Token|
|/blogs|GET|NO|null|List Of Blogs|
|/blogs|POST|YES|new Blog|new Blog|
|/blogs/:id|GET|NO|null|Blog|
|/blogs/:id|DELETE|YES|null|null|
|/blogs/:id|UPDATE|YES|new Blog|new Blog|
|/user|GET|YES|null|List of all users|
|/user/:id|GET|YES|null|user|
|/user/:id|DELETE|YES|null|user|
|/products|GET|NO|null|List of products|
|/products|POST|YES|new product|new product|
|/products/:id|GET|NO|null|product|
|/products/:id|DELETE|YES|null|deleted product|
|/products/:id|UPDATE|YES|updated product|updated product|

---

|Endpoint|Method|Protected|Body|Response|
|-|-|-|-|-|
|/order|GET|YES|null|all orders by user|
|/order|POST|YES|order|new order|
|/order/:id|GET|YES|null|order|
|/order/:id|DELETE|YES|null|order|
|/order/:id|UPDATE|YES|order|order|
