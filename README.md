User Reviews Functionality for Drupal Website
-
Introduction
-
This Project enhances a Drupal website by adding user reviews functionality, enabling registered users to submit reviews for products listed on the site. The process involves creating a custom content type for products, setting up review fields, configuring permissions, and optimizing the display of reviews. Additionally, the Project includes features for moderation and performance optimization.

Features
-
Content Type Setup
-
1) Review Comment Type: A comment type named "Review" is created to capture user reviews. It includes fields for the comment itself and a rating (1 to 5 stars).
2) Product Content Type: A custom content type named "Product" is created to represent individual products listed on the website. It includes fields for description, image, and an "Add to Cart" button, and add review(comment type) functionality.

Permissions
-
1) User Access Control: User permissions are configured to ensure that all users, including anonymous ones, can view the product listing without logging in. However, only authenticated users can access the review section to submit reviews.

2) Administrator Approval: Reviews are subject to moderation, with only approved reviews being displayed on the site. Administrators have the authority to approve or reject reviews before they become visible to other users.

Review Display
-
1) Sorting: Reviews are displayed on product pages in descending order based on submission time, ensuring that the newest reviews appear first. This feature is achieved using the "Comment Order" contributed module.

2) View Integration: A view is created to display all products listed on the website. This view provides users with an organized overview of available products and facilitates navigation to individual product pages for reviewing.

Captcha Integration
-
Enhanced Security: To enhance security and prevent spam, a CAPTCHA is implemented on the user login form. This feature is achieved through the integration of the "CAPTCHA" contributed module, providing an additional layer of authentication.

Code Flow
-
1) User Interface:-
   -
    Users access the Drupal website and navigate to the "product" menu without needing to log in, where they can view the list of available products.

2) Review Submission:-
   -
   1. Upon finding a product they wish to review, users must log in to access the review section.
   2. Once logged in, users can submit reviews by providing a comment and rating in the review submission form.

3) Moderation:-
   -
   1. Submitted reviews are not immediately visible on the site. Instead, they enter a moderation queue.
   2. Administrators review the submitted reviews and approve or reject them accordingly.
   3. Only approved reviews are displayed on the product page, with the newest reviews shown first.

Installation
-
Clone Repository:
-
Clone a project repository from GitHub "https://github.com/SoumySoni/OrangeMantra" to your server environment where Drupal 10 is installed.

Database Import:
-
Import the "review_database" file into your Drupal 10 database management system.
