*** Task 16: Creating a database ***

Database IMDB is created:

![Alt text](image.png)

Create table : Artist

Query: CREATE TABLE Artist(artist_id INT PRIMARY KEY, artist_name VARCHAR(100), gender VARCHAR(20));

![Alt text](image-1.png)

Create table : Artist Skill Set

Query: CREATE TABLE Artist_skill_set(skill_id INT PRIMARY KEY, skill_name VARCHAR(100), artist_id INT, FOREIGN KEY (artist_id) REFERENCES artist(artist_id));

![Alt text](image-2.png)

Create table: Skills
Query:  CREATE TABLE Skills(skill_id INT PRIMARY KEY, skill_name VARCHAR(100));

![Alt text](image-3.png)

Create table: user
Query:  CREATE TABLE user(user_id INT PRIMARY KEY, user_name VARCHAR(100));

![Alt text](image-4.png)

Create table: media
Query: CREATE TABLE Media(media_id INT AUTO_INCREMENT PRIMARY KEY, media_type VARCHAR(100), movie_id INT, FOREIGN KEY (movie_id) REFERENCES Movie_Details(movie_id));

![Alt text](image-5.png)

Create table: Genre 
Query:  CREATE TABLE genre(genre_id INT PRIMARY KEY, genre_type VARCHAR(100), movie_id INT, FOREIGN KEY (movie_id) REFERENCES Movie_Details(movie_id));

![Alt text](image-6.png)

Create table: Review
Query:  CREATE TABLE reviews(review_id INT PRIMARY KEY, review VARCHAR(1000), user_id INT, FOREIGN KEY (user_id) REFERENCES user(user_id), media_id INT, FOREIGN KEY (media_id) REFERENCES Movie_details(movie_id), rating VARCHAR(100));

![Alt text](image-7.png)

Create table: Atrist role
Query: CREATE TABLE artist_role(role_id INT PRIMARY KEY, role_name VARCHAR(100), artist_id INT, FOREIGN KEY (artist_id) REFERENCES artist(artist_id), movie_id INT, FOREIGN KEY (movie_id) REFERENCES movie_details(movie_id));
![Alt text](image-8.png)

Create table: Movie details
Query: 



Insert data in user table:
![Alt text](image-9.png)

Insert data in skills table:
![Alt text](image-10.png)

Insert data in artist table:
![Alt text](image-11.png)

