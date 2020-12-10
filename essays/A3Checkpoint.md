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
 
Since session are unique to a user, I can use a session to keep track of each user is saving to their cart. This data should not overwrite since each user has a specific session ID.

I will also use sessions to keep track of the user’s shopping cart and store the shopping data to the session. Session data does not change unless it is destroyed, or the server is restarted so the data will transfer to the invoice. When the user checks out, the session data will be requested to write the invoice.

Checkpoint C:
How will you avoid access to your application when the user has not logged in or registered? What are the particular security concerns you must address?
 
I can give the user a cookie once they log in. Since the cookie data is saved while moving through pages, when it is time to log out, I can request the cookie from the user. If there is not cookie, I will redirect the user to re-login. If there is a cookie the user can proceed to check out. To handle the security issues, I will set the cookie to expire. Since cookies are easily tampered with, I will make encrypt the cookie.
 
Checkpoint D:
Upon successful login, how do you provide personalization in your UI? Explain how you did or will do this (paste code if necessary):
 
Upon successful login, I plan to personalize my UI by display a “Thank you username for!” and a “Thank you username for your purchase message!.... A copy of the invoice has been sent to you at email.” To do this, I will mainly be storing the request.body.username in a variable and obtaining the email address from the username in the user_reg_info.json.

Checkpoint E:
If you are working with partners, how will you split up the work in your team so that you are working in parallel as effectively as possible? That is, who is doing what and when?
 
I will not be working with a partner for Assignment 3.
 
Checkpoint F:
How are you approaching Assignment 3 differently than Assignment 2?

I am approaching Assignment 3 differently than I approach Assignment 2 since I have created a prototype for Assignment 3 already. I think that this has already helped me to be more organized and brainstorm how I would like to format and code the website. From making the prototype, I also know that I would like to add more product variety to my original design. In Assignment 2, I planned my code while working on it so I would get a lot of unexpected errors and waste a lot of time.
