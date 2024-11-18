# Instagram-Database-Clone
Here’s a professional README template for creating an Instagram database clone using MySQL, inspired by Colt Steele's Udemy course:  

---

# Instagram Database Clone using MySQL

## 📖 Overview  
This project replicates the database structure of Instagram, focusing on creating tables, relationships, and constraints to model the platform's core functionalities. The implementation is based on the **Udemy course by Colt Steele**.  

## 🚀 Features  
- User accounts with detailed profiles.  
- Posts, including captions and timestamps.  
- Comments on posts.  
- Follower-following relationships.  
- Likes for posts.  
- Real-world database constraints (e.g., primary keys, foreign keys, unique constraints).  

## 🛠️ Technologies Used  
- **MySQL**: For database management.  
- **SQL**: To write and execute queries.  
- **Workbench/CLI**: To interact with MySQL.  

## 📚 Learning Outcomes  
By following this project, you will learn to:  
- Design and normalize relational databases.  
- Use MySQL to create, manage, and query tables.  
- Implement many-to-many and one-to-many relationships.  
- Apply constraints to ensure data integrity.  
- Understand real-world database schema design concepts.  

## 🗂️ Database Schema  
The database consists of the following tables:  
1. **Users**  
   - Fields: `id`, `username`, `email`, `password`, `profile_picture`, `created_at`  
2. **Posts**  
   - Fields: `id`, `user_id`, `caption`, `image_url`, `created_at`  
3. **Comments**  
   - Fields: `id`, `post_id`, `user_id`, `comment_text`, `created_at`  
4. **Likes**  
   - Fields: `id`, `post_id`, `user_id`, `created_at`  
5. **Followers**  
   - Fields: `follower_id`, `following_id`  

### Relationships  
- Users ↔ Posts (1:N)  
- Users ↔ Followers (N:M via `Followers` table)  
- Posts ↔ Comments (1:N)  
- Posts ↔ Likes (1:N)  

## 🔄 Workflow  
1. **Schema Design**: Using MySQL, create the necessary tables with constraints.  
2. **Insert Data**: Populate tables with dummy data to test relationships.  
3. **Query Testing**: Run queries to retrieve meaningful insights like:  
   - Fetch all posts by a specific user.  
   - Retrieve all followers of a user.  
   - List the most-liked posts.  

