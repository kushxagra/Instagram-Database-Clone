This project involves creating an Instagram database clone by designing and implementing a relational database using MySQL. 
The database design is based on concepts taught in Colt Steele’s Udemy course, "The Ultimate MySQL Bootcamp." 
The project models core Instagram functionalities, including user accounts, posts, comments, likes, and follower relationships, using normalized database structures with appropriate constraints and relationships.

The database consists of multiple tables:

    Users: This table stores information about user accounts, including fields such as id, username, email, password, profile_picture, and created_at.
    Posts: This table records the posts made by users, including fields such as id, user_id, caption, image_url, and created_at.
    Comments: This table stores comments on posts, with fields such as id, post_id, user_id, comment_text, and created_at.
    Likes: This table tracks likes on posts, with fields such as id, post_id, user_id, and created_at.
    Followers: This table manages follower-following relationships between users, with fields follower_id and following_id.

The database implements relationships such as one-to-many (Users to Posts, Posts to Comments, Posts to Likes) and many-to-many (Users to Followers through the Followers table).
These relationships are enforced through the use of primary keys, foreign keys, and other constraints to maintain data integrity.
