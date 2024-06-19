# 1. Data Dive (10 pts):
The data i choose was Social Media Users

# Difficulties
Data Cleaning and Consistency: One of the primary challenges was ensuring the consistency and cleanliness of the data. For instance, the interest category "Lifestlye" seems to be a typographical error and should be corrected to "Lifestyle".

Gender Diversity: The dataset includes non-binary gender categories, which is important for inclusivity but can be challenging if not all analysis tools support this category effectively.



## Interesting Observation
One interesting observation from the dataset is the distribution of social media platform usage among different professions and interests. For example, individuals interested in "Sports" predominantly use "Instagram," whereas those interested in "Lifestyle" and "Travel" have a more balanced usage across "YouTube" and "Facebook". This could suggest that "Instagram" has a stronger appeal to sports enthusiasts, which might be valuable information for targeted marketing strategies.


## 2. Data Fun (20 pts)
Use simple SQL queries to play with the data.
Find 2 cool facts hidden within the data (e.g., most popular interests).

SELECT interests, COUNT(*) AS age
FROM users
GROUP BY interests
ORDER BY age DESC
LIMIT 1;

Use basic SQL queries like (COUNT, AVG, and SUM) to understand more about the data you have.

Average Age of Users:
SELECT AVG(age) AS average_age
FROM users;
 answer = 40.9860

Gender Distribution:
SELECT gender, COUNT(*) AS num_users
FROM users
GROUP BY gender;

Top Occupations:
SELECT occupation, COUNT(*) AS num_users
FROM users
GROUP BY occupation
ORDER BY num_users DESC
LIMIT 3;



## 3. Ask Away (30 pts):

Formulate 2 questions about the data (e.g., what are popular shows in different countries?).

1. What are the top three most common occupations among female users?
2. How many non-binary people own a home 

Write basic SQL queries (WHERE, ORDER BY) to find answers.
Share what you learned from the answers.
answer 1
SELECT profession, COUNT(*) AS num_users
FROM time
WHERE gender = 'Female'
GROUP BY profession
ORDER BY num_users DESC
LIMIT 3;

results
	
Software Engineer
115
Student
108
Marketer Manager
108





