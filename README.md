# Book_Store_Web_App
 BOOK STORE application is a Maven Project based on the Model-View-Controller (MVC) software design pattern to develop user interface application for customers to purchase books online. It is secure, restful ecommerce website which is used to order the books online by customers and get products on the door within few hours.

 Technologies used: Frontend: Angular , Bootstrap
                   Backend : Spring Boot , Hibernate
                   Database: MySql

FrontEnd Description:
                  Headers:  For All ( Home, All Products, Book List, About us)
                            For User/Customer ( Home, All Products, Book List, About us, Cart, My Orders)
                            For Admin ( Home, All Products, Book List, About us, Add Products, Product Details, All Orders, All Users)

Backend Description: 
                  Modules:  Role, User, Admin, Product, Order, Cart, ImageModel, TransactionDetails
                  
                  Controller-> Service-> Repository/Dao-> Database-> Entity/Model

User Role Flow :- 1) User will create their account and user details will store to database
                  2) User will login through their credentials, which will be authenticated using Jwt token.
                  3) After successful login, User dashboard will be displayed 
                      user can- i.   View products
                                ii.  View product details
                                iii. Add products to the cart
                                iv.  Buy products 
                                v.   During checkout, Customer has to fill the form having details like name, address, phone no.
                                vi.  Pay bill by razorpay online
                                vii. View Order details in my orders and order status (placed or delivered)

                                
Admin Role Flow :- 1) By default one admin has been created 
                   2) Admin will login through their credentials, which will be authenticated using Jwt token.
                   3) After successful login, Admin dashboard will be displayed 
                        admin has access to - i.   Add Books(Book name, book description, price, images)
                                              ii.  View book details and can update book details
                                              iii. View all the orders (placed, delivered) and mark the products as delivered 
                                              iv.  View all the users 

Security :- Spring security Jwt Token has been used for authentication and give authorization access to the api according to their role(User/Admin)

Payment  :- RazorPay payment gateway has been used for online payment
