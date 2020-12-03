---
layout: essay
type: essay
title: Checkpoint Assignment 3
date: 2020-12-03
labels:
  - Blog
  - Assignment 3
---

Checkpoint A:
Describe your design for your site's shopping cart. That is, will it be a separate page that the user can view and edit, or will it be integrated into the product pages? If so, describe in detail how this will work on your site. Provide several examples of using the cart.
 
Since the majority of my pages, the invoice, login, and registration pages are generated on the server, I plan to do the same with my cart and product pages. I plan to have to cart be accessible to users in the navigation bar. The way they add to the cart is by using the “Add to cart” button on one of the product pages.
 
For example, a user who wants to order 3 diamond necklaces would go to the diamond necklace page select 3 then press “Add to Cart”. Next, they would go to “cart” through the navbar check the amount, and press “proceed to checkout” which would then prompt them to log in.
 
Checkpoint B:
Explain specifically how you will use sessions to manage your shopping cart. In particular, what shopping cart data will be stored in the session, what data format will be used (NOT what data type, but the format like with the data format used for your registration data). Use code examples showing what data structures (such as arrays and their keys) you will use to manage the shopping cart data and how they will be used in $_SESSION.
 
I will be using sessions to enable multiple users to order at once. One of the potential issues with my code from Assignment 2 was that the user’s product selections would overwrite. So I will use a session to prevent the cart from being overwritten. The example from Assignment 3 used a session and requested the info from the session.  
 
Checkpoint C:
How will you avoid access to your application when the user has not logged in or registered? What are the particular security concerns you must address?
 
My main concern is to prevent users who do not have an account from ordering products/accessing the invoice page. To prevent this, I have a function that only displays the invoice if the login/registration is valid. The main concern is preventing people from accessing the invoice by just adding the proper URL string. Additionally, a potential problem that I have from assignment 2 is that the user’s product selection would be overwritten by the next user, so preventing that using sessions would be important.
 
Checkpoint D:
Upon successful login, how do you provide personalization in your UI? Explain how you did or will do this (paste code if necessary):
 
Upon successful login, I plan to personalize my UI by display a “Thank you username for!” and a “Thank you username for your purchase message!.... A copy of the invoice has been sent to you at email.” To do this, I will mainly be storing the request.body.username in a variable and obtaining the email address from the username in the user_reg_info.json.
 
Checkpoint E:
If you are working with partners, how will you split up the work in your team so that you are working in parallel as effectively as possible? That is, who is doing what and when?
 
I will not be working with a partner for Assignment 3.
 
Checkpoint F:
How are you approaching Assignment 3 differently than Assignment 2?

I am approaching Assignment 3 differently than I approach Assignment 2 since I have created a prototype for Assignment 3 already. I think that this has already helped me to be more organized and brainstorm how I would like to format and code the website. From making the prototype, I also know that I would like to add more product variety to my original design. In Assignment 2, I planned my code while working on it so I would get a lot of unexpected errors and waste a lot of time.
