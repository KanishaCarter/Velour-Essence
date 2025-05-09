# velour-essence
Capstone Project
Unit 5
 
 
Lesson Overview
In this lesson, we will learn about the capstone project we will build to put all our knowledge into practice. We will use this lesson to get organized and start planning!

Pro-Tip: You will want to discuss and display this on your resume and in interviews.

Capstone Learning Objectives
Create a pull request on GitHub; use the GitHub interface to accept and merge it.
Use the GitHub interface to code review a pull request.
Use Git to resolve merge conflicts.
Create a full stack application
Instructions:
The capstone project is your opportunity to demonstrate your Web Development skills by creating a full stack application. You will work individually to create an application, including all the MVP features and adding as many extra features as time allows.

If you want to work in a team,  you will need to gather your desired team members, fill out a provided application, and submit it to your instructor for approval. If you work in a group, you will work together to create an e-commerce site selling items of your choice, but it will be more difficult as you will need to implement more features.

Once you make your choice, you should look closely through the product requirements and determine which features you would like to implement.

For all projects, Tier 1: MVP is required. An MVP, or Minimum Viable Product, describes the absolute minimum features a product needs to be usable for its main purpose. Tiers 2 and 3 for each project describe more complex, useful, or design-oriented features that improve a product's chances in the market.

Your may choose any, all, or none of the features in Tiers 2 or 3 to implement, but choose wisely. Once your project deadline is reached, you must present a working website with some working features to demonstrate to your fellow learners and instructional team members.

Read the instructions and your option's requirements carefully, and use the lesson resources as needed. 

There are four tabs below. Read the instructions and your option's requirements carefully, and use the lesson resources as needed. 

Lesson ResourcesApplication RequirementsDeliverables
E-Commerce App
Tier 1: MVP (Minimum Viable Product)
AS A USER (NOT LOGGED IN), I SHOULD BE ABLE TO:
Access the website via the internet so I can browse and purchase products.
View all available products.
View the details for an individual product, including product descriptions, photos, price, etc.
If I do not have an account, create an account.
If I do have an account, log into my account.
AS A USER (LOGGED IN), I SHOULD BE ABLE TO:
Have a persistent cart to revisit and pick up where I left off.
For example, I am logged in on my mobile device and add some items to my cart. When I open the browser on my laptop and log in, I want to see those items in my cart.
No one else should be able to edit my cart except me.
Add a product to my cart.
Edit my cart if I change my mind:
Change the quantity of a product in my cart.
Remove a product from my cart.
No one else should be able to edit my cart except me.
"Check out" the items in my cart, i.e., purchase the products.
Think of the user experience when checking out on a typical e-commerce site like Amazon, etc.
You can start by simulating the experience of checking out with a simple confirmation page.
AS AN ADMINISTRATOR, I SHOULD BE ABLE TO:
View a list of all products.
Add, edit, and remove products.
No one else should have access.
View a list of all users.
This list should include all relevant user information.
This could include name, email address, mailing address, phone number, billing information, etc.
AS AN ENGINEER, I SHOULD:
Have a well-seeded database so that I can simulate several different scenarios for the user stories below.
By doing this, you set yourselves up to tackle many of the points throughout the tiers. In the long run, this will potentially save you tons of time.
For example, seed hundreds of products with dummy data so that when you get to the “pagination” user story, you will not have to worry about adding more products.
Likewise, add a bunch of users with products in their carts so editing the cart can be worked on without already having the “add to cart” functionality built out.
Have secured user data so that no one can unrightfully manipulate information.
TIER 2: E-Commerce Essentials
AS A USER (NOT LOGGED IN), I WANT TO BE ABLE TO:
Sort products by certain characteristics.
This could be name, price, etc.
Filter products by certain characteristics.
This could be category, type, maximum/minimum price, etc.
Enjoy an aesthetically pleasing website that is intuitive and easy to use (UI/UX).
Be able to use all website features whether I am using a phone, tablet, or laptop/desktop computer.
Navigate the website successfully regardless of disability.
This is a great opportunity to dive into ADA Compliance (screen-reader friendliness, keyboard navigation, colorblind-friendly, etc.).
Resources: A11y ChecklistLinks to an external site., WebAIM Contrast CheckerLinks to an external site.
Know when content is loading, or if there is an error, so I can manage my expectations.
Examples:
Show loading indicators while the frontend is waiting for a backend response.
If I visit a product page that does not exist, notify me and give me a link to go to a list of all products or back to the previous page.
Have a persistent shopping cart to revisit and pick up where I left off.
There are two more experiences to consider here. Explore your favorite websites to see what the intended behavior is for the following cases:
Guest-only: I do not want to create an account, but I want my cart to persist between browser refreshes.
Guest-to-logged-in-user: Initially, I am not logged in, and I add items to my cart. When I eventually log in, I want to see those same items I added when I was logged in still in my cart, in addition to the items I may have had in my cart from a previous logged-in session.
AS A LOGGED-IN CUSTOMER, I SHOULD BE ABLE TO:
See my order history to remember my previously purchased items and their prices at the time of purchase.
View and edit my user profile so I can update my information when necessary.
AS AN ADMINISTRATOR, I SHOULD BE ABLE TO:
Have access to a dashboard with the following functionality:
Create and edit products with name, description, price, and one or more photos.
Create and manage categories or tags for products to allow for more useful searches and filters.
Manage the stock status or quantity of a product, thereby controlling whether or not a user can purchase that product.
View a searchable list of all orders that can also be filtered by status, for example: Created, Processing, Cancelled, Completed.
Modify the order status (Created -> Processing, Processing -> Cancelled || Completed), so that others will know what stage of the process the order is in.
Promote other user accounts to have administrator status.
Modify and delete other user accounts.
Allow customers to have a variety of payment method options to increase checkout conversion.
Begin by integrating Stripe.
For the client side, use Stripe's prebuilt CheckoutLinks to an external site. form, ideally with the "Custom" strategy. We recommend react-stripe-checkoutLinks to an external site. in this case. Build a custom form and communicate with Stripe and your server via Stripe.jsLinks to an external site..
For the server side, use the [stripe](<https://stripe.com/docs/libraries#node-library>) npm library (API docs hereLinks to an external site., tutorial hereLinks to an external site.) to accept tokens from your front-end app and send charges via the Stripe API.
TIER 3: Extra Features
AS A CUSTOMER (NOT LOGGED IN), I SHOULD BE ABLE TO:
Log in through third-party authentication to avoid creating an account specific to the website. For example, Google OAuth.
AS A CUSTOMER (LOGGED IN), I SHOULD BE ABLE TO:
Create a wish list of products I want to buy.
Be able to share a wish list link with other users.
Add products from another user’s wish list to my cart and purchase them.
Have products removed or marked on my wish list if they are purchased by another user with my wish list.
Receive notifications, either by email or on the site, for the following actions or events:
I placed an order.
Item(s) from my wish list were purchased by another user.
View items and reviews in a more user-friendly way:
More advanced search and filter options
Pagination
Infinite scrolling, i.e., more products appear when you scroll to the end of the page.
Receive recommendations for items based on my reviews.
For example, if I purchased a product from a certain category, I might see recommendations for other products from the same category.
AS AN ADMINISTRATOR, I SHOULD BE ABLE TO:
View information about a users’ wish lists from my dashboard.
Trigger a password reset for a user (that is, the next time they successfully log in with their old password, they are prompted for a new one), so that I can be proactive in getting users to change their passwords after a period of time.
Allow stock quantity to be tied to orders.
When a customer purchases an item, the quantity available is appropriately deducted.
Likewise, if a customer attempts to purchase a higher quantity of an available item, they will be alerted/notified that there is not enough inventory.
