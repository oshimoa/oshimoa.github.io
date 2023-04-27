---
layout: essay
type: essay
title: "Checkpoint Assignment #3"
# All dates must be YYYY-MM-DD format!
date: 2023-04-26
published: true
labels:
  - ITM 352
  - Checkpoint
  - Assignment3
---

Presentation: https://youtu.be/ES2mQ50Vp-c

**Show what each page will look like. The pages do not have to be “functional” but the design should be clear.** <br>
Discussed in the presentation.<br>
**Describe your design for your site’s shopping cart. That is, will it be a separate page that the user can view and edit, or will it be integrated into the product pages? If so, describe in detail how this will work on your site. Provide several examples of using the cart.**<br>
I have a separate page for the cart so that users can update the quantity that they desire. In the Quantity textbox, they can input a new value and click update cart to post these changes. On the storepage with the products, when they click add to cart, the values are collected in an array and posted to the cart page. <br>
**Explain specifically how you will use sessions to manage your shopping cart. In particular, what shopping cart data will be stored in the session, what data format will be used (NOT what data type, but the format like with the data format used for your registration data). Use code examples showing what data structures (such as arrays and their objects) you will use to manage the shopping cart data and how they will be used in a session.**<br>
Here, I use sessions to store the data about the products quantity, name, and picture in an array that will be saved in a session for my cart. Then, the server can retrieve the session data associated with the user's session ID since users have to login in before accessing their cart, and use it to display the selected items in the cart. When the user proceeds to the invoice or checkout page, the server can use the session data to calculate the total cost, and generate the invoice based on the cart contents stored in the session data. This can allow the server to store and retrieve the selected items in the cart for each user's session. Code shown in presentation.<br>
**How will you avoid access to your application when the user has not logged in or registered? What are the particular security concerns you must address?**<br>
This is some code that I have in my cart file which basically sees if a user is logged in by using cookies to recall the user’s name and if there is no cookie with the name, then users must log in. Some security concerns would be people not entering necessary information to complete a purchase and send an invoice like their email address. Also another concern would be people anonymously editing product data and affecting quantities available. Another concern is storing passwords and sensitive information encrypted. Code shown in presentation.<br>
**Upon a successful login, how do you provide personalization in your UI? Explain how you did or will do this (paste code if necessary).**<br>
The user interface has personalization on the cart, products, and invoice page which all display the user’s name. I do this by using a get cookie to get the user’s name after they sign in. Code shown in presentation.<br>
**If you are working with partners, how will you split up the work in your team so that you are working in parallel as effectively as possible? That is, who is doing what and when?**<br>
I will be working with one partner and since Assignment 3 is based on my original store, I did a lot of the initial work to get Assignment 3 going like setting up the cart and adding product pages. My partner will be working on the admin back end and IRs since they are tasks that come in a little later and are easier to add in without disturbing the main architecture too much. I did most of the work earlier on because I am going to be working a lot of shifts during finals week between my two jobs and my partner is starting now that I have set up Assignment 3.<br>
**How are you approaching Assignment 3 differently than Assignment 2?**<br>
I am approaching Assignment 3 differently in that I focused more on outlining what needed to be done with comments first instead of just trying to go task by task. This was a lot  more efficient since I got a broader perspective.<br>
