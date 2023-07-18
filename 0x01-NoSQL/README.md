# NoSQL Project

This project contains a set of scripts and functions related to MongoDB and NoSQL databases. The scripts perform various operations on MongoDB collections and provide useful information and functionality.

## Usage

### 0. List all databases

Script: `0-list_databases`

This script lists all databases in MongoDB.

### 1. Create a database

Script: `1-use_or_create_database`

This script creates or uses the database `my_db` in MongoDB.

### 2. Insert document

Script: `2-insert`

This script inserts a document with the name "Holberton school" into the `school` collection.

### 3. All documents

Script: `3-all`

This script lists all documents in the `school` collection.

### 4. All matches

Script: `4-match`

This script lists all documents with the name "Holberton school" in the `school` collection.

### 5. Count

Script: `5-count`

This script displays the number of documents in the `school` collection.

### 6. Update

Script: `6-update`

This script adds a new attribute "address" with the value "972 Mission street" to all documents with the name "Holberton school" in the `school` collection.

### 7. Delete by match

Script: `7-delete`

This script deletes all documents with the name "Holberton school" in the `school` collection.

### 8. List all documents in Python

Script: `8-main.py`

This Python script lists all documents in the `school` collection using the `list_all` function.

### 9. Insert a document in Python

Script: `9-main.py`

This Python script inserts a new document into the `school` collection using the `insert_school` function.

### 10. Change school topics

Script: `10-main.py`

This Python script changes the topics of a school document based on the name using the `update_topics` function.

### 11. Where can I learn Python?

Script: `11-main.py`

This Python script returns a list of schools that have a specific topic using the `schools_by_topic` function.

### 12. Log stats

Script: `12-log_stats.py`

This Python script provides statistics about Nginx logs stored in MongoDB, including the number of logs, HTTP methods, and status checks.

### 100. Regex filter (advanced)

Script: `100-find`

This script lists all documents with names starting with "Holberton" in the `school` collection.

### 101. Top students (advanced)

Script: `101-main.py`

This Python script returns all students sorted by average score using the `top_students` function.

### 102. Log stats - new version (advanced)

Script: `102-log_stats.py`

This improved version of the log stats script includes the top 10 most present IP addresses in the `nginx` collection of the `logs` database.
