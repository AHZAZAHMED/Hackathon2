# 🚀 Hackathon Day 2: Technical Foundation Successfully Completed!

It was another productive day at the Hackathon as I wrapped up Day 2, focusing on Technical Planning and System Architecture for our e-commerce platform. The day was dedicated to establishing the foundation for a scalable, efficient, and high-performance system!

## 1️⃣ Defining Technical Requirements 🛠️
- ### Frontend Requirements:
 #### Framework:
   Use Next.js to build a fast, SEO-friendly, and scalable frontend.

#### User Interface:
- Design a user-friendly interface to allow seamless browsing of products.
- Optimize the interface for easy navigation and a smooth shopping experience.
#### Responsive Design:
Ensure the website is fully responsive, providing an excellent user experience across mobile, tablet, and desktop devices.

#### Essential Pages:
 - Homepage: Highlight featured products, categories, and promotions.
- Product Listing Page: Display all available products with filters (e.g., price, category).
- Product Details Page: Provide detailed information about a selected product, including images, descriptions, and reviews.
- Cart Page: Allow users to view selected items, update quantities, and remove products.
- Checkout Page: Collect shipping and payment details.
- Order Confirmation Page: Display order details and confirmation after successful payment.

- ### Backend & Database (Sanity CMS):

Use Sanity CMS to act as the backend database, managing:
- Product Data: Add, update, or delete products dynamically.
- Customer Details: Store user profiles, login information, and addresses.
- Order Records: Track orders, payment statuses, and shipping details.


 Relationships Diagram Between Entities:

[Relationship Diagram](https://app.eraser.io/workspace/1hbFgpQdVBOi5E720VVw)

- ### Third-Party API Integration
- Shipment Tracking API:Integrate a shipment tracking service to provide users with real-time order tracking.Display tracking updates on the Order Confirmation Page or via user profile.

- Payment Gateway:Use APIs like Stripe for secure payment processing.Handle multiple payment methods (e.g., credit/debit cards, online wallets).

## 2️⃣ Design System Architecture

System Architecture Diagram:

[Diagram](https://app.eraser.io/workspace/1hbFgpQdVBOi5E720VVw)

 ## 3️⃣ Plan API Requirements 

 1  Endpoint Name: /products
  - Method: GET
 - Description: Fetch all available products from Sanity.
 - Response: Product details (ID, name, price, stock, image).

2 Endpoint Name: /cart_items
-  Method:POST
- Descriptions: Add item to the cart
- Response: Product details (ID, name, price, image)

3 Endpoint Name: /cart_items
-  Method:GET
- Descriptions: Fetch item details form the cart
- Response: Product details (ID, name, price, image)

4 Endpoint Name: /order_detail
-  Method: POST
-  Description: Create a new order in Sanity.
-  Payload: Customer info, product details, payment status. 

5 Endpoint Name: /payment_detail
- Method: GET
- Description: Fetch all payment detail form sanity.

6 Endpoint  Name: /shipment_detail
- Method:GET
- Description: Fetch allshipment detail  form sanity.
 Response: delivery status,delivery date,customer info