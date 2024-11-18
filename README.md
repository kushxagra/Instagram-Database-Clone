This project involves designing and implementing a relational database in MySQL to replicate core Instagram functionalities. 
The database models key features like user accounts, posts, comments, likes, and follower relationships, based on concepts from Colt Steele’s "The Ultimate MySQL Bootcamp".

Key Features:

Users: Stores user information (id, username, email, password, profile picture, etc.).
Posts: Tracks user posts (id, user_id, caption, image_url, etc.).
Comments: Stores comments on posts (id, post_id, user_id, comment_text, etc.).
Likes: Tracks likes on posts (id, post_id, user_id).
Followers: Manages follower-following relationships between users.
Database Design:
One-to-Many: Users to Posts, Posts to Comments, Posts to Likes.
Many-to-Many: Users to Users (via Followers table for follower-following relationships).
The database ensures data integrity through normalized structures, primary keys, foreign keys, and other constraints.
