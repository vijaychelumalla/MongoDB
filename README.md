#   MongoDB Intern Training Guide (Beginner to Intermediate)

This repository contains my MongoDB internship training tasks and practice exercises completed using the **sample_mflix** database. The objective of this training was to build a strong foundation in MongoDB concepts, CRUD operations, query operators, update operators, and data retrieval techniques through hands-on practice.

---

##    Topics Covered

### MongoDB Fundamentals

Introduction to MongoDB
Documents vs Collections
BSON Basics
Nested Documents
Arrays in MongoDB
Understanding the sample_mflix Database

### CRUD Operations

insertOne()
insertMany()
find()
findOne()
updateOne()
updateMany()
deleteOne()
deleteMany()

### Query Operators

$eq, $ne
$gt, $gte, $lt, $lte
$in, $nin
$and, $or
$exists
$regex
$all, $size, $elemMatch

### Update Operators

$set
$unset
$inc
$push
$pull
$addToSet

### Cursor Operations

sort()
limit()
skip()
Projection

---

## ⚙️ How to Run Queries

### Using MongoDB Compass

1. Open MongoDB Compass and connect to your Atlas Cluster.
2. Open the sample_mflix database.
3. Select the required collection (for example, movies).
4. Navigate to the **Documents** tab.
5. Enter the query in the filter box.

Example:

javascript
{ year: { $gt: 2000 } }



This query returns all movies released after the year 2000.

6. Click **Find** or **Apply** to execute the query.

### Using Mongo Shell


javascript
use sample_mflix

db.movies.find({
    year: { $gt: 2000 }
}).pretty()



Use .pretty() for better output formatting.

---

##    Important Guidelines

Create a separate file for each practice question.
Include the question number in the filename.
Write the question statement at the top of the file.
Add the MongoDB query below the question.
Execute and verify queries in MongoDB Compass before submission.
Save all practice queries for future revision.
Validate the output before final submission.

---

##   Practice Questions (sample_mflix)

### Basic Queries

1. Find all movies.
2. Find the first movie document.
3. Find movies released after 2000.
4. Find movies released before 1990.
5. Find movies with runtime greater than 120 minutes.
6. Find movies with runtime less than 90 minutes.
7. Find movies with genre "Drama".
8. Find movies with genre "Comedy".
9. Find movies with IMDb rating greater than 8.
10. Count the total number of movies.

### Working with Collections

11. Find comments by a specific user.
12. Find movies from a specific country.
13. Find movies in a specific language.
14. Find theaters in a specific city.
15. Find movies released in a specific year.
16. Find movies between two years.
17. Find movies with runtime between two values.
18. Find movies with rating greater than X and runtime greater than Y.
19. Find movies having both Drama and Comedy genres.
20. Find movies with a missing poster field.
21. Find movies where awards.wins is greater than 5.
22. Return only title and year fields.

### Cursor Operations

23. Sort movies by year in ascending order.
24. Sort movies by year in descending order.
25. Return the top 10 newest movies.
26. Return the first 20 movies.
27. Skip the first 20 movies and return the next 20.

### Update Operations

28. Update a movie runtime.
29. Update a movie title.
30. Add a new field into a document.
31. Increase a numeric field using increment.
32. Remove a field from a document.

### Delete Operations

33. Delete one comment.
34. Delete multiple comments.

### Insert Operations

35. Insert one movie document.
36. Insert multiple movie documents.

### Advanced Queries

37. Find movies using regex on the title.
38. Find movies where the cast contains a specific actor name.
39. Find movies with more than one country.
40. Find movies having at least three genres.
41. Find documents using the OR condition.
42. Find documents using the AND condition.
43. Find movies with a specific language and genre.
44. Add an item into an array using $push.
45. Remove an item from an array using $pull.

---

## Learning Outcomes

By completing these exercises, I gained practical experience in:

MongoDB database fundamentals
Querying and filtering documents
Performing CRUD operations
Using query and update operators
Working with arrays and nested documents
Implementing pagination techniques
Managing data efficiently using MongoDB Compass and Mongo Shell
Writing optimized MongoDB queries

---

### Database Used

**Database:** sample_mflix

This sample dataset provided real-world movie-related data to practice MongoDB concepts and strengthen database skills through hands-on exercises.
