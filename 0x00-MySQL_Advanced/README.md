# 0x00-MySQL_Advanced

This repository contains SQL scripts for various tasks related to advanced MySQL concepts. Each task is described below along with the corresponding script file.

## Task 0: We are all unique!

- Script: `0-uniq_users.sql`
- Description: Creates a table named `users` with the specified attributes (`id`, `email`, and `name`). The `email` attribute is set to be unique, and the script ensures that the table is not created if it already exists.

## Task 1: In and not out

- Script: `1-country_users.sql`
- Description: Creates a table named `users` with additional attribute `country`. The `country` attribute is an enumeration of countries (`US`, `CO`, and `TN`), and its default value is `US`.

## Task 2: Best band ever!

- Script: `2-fans.sql`
- Description: Ranks the country origins of bands based on the number of fans. It uses a pre-imported table dump named `metal_bands.sql.zip`.

## Task 3: Old school band

- Script: `3-glam_rock.sql`
- Description: Lists all bands with "Glam rock" as their main style, ranked by their longevity. It uses a pre-imported table dump named `metal_bands.sql.zip`.

## Task 4: Buy buy buy

- Script: `4-store.sql`
- Description: Creates a trigger that decreases the quantity of an item after adding a new order. It demonstrates how to maintain data integrity by updating multiple tables using triggers.

## Task 5: Email validation to sent

- Script: `5-valid_email.sql`
- Description: Creates a trigger that resets the `valid_email` attribute only when the email has been changed. It shows how to distribute the logic of email validation to the database itself.

## Task 6: Add bonus

- Script: `6-bonus.sql`
- Description: Creates a stored procedure named `AddBonus` that adds a new correction for a student. The procedure takes three inputs (`user_id`, `project_name`, and `score`) and handles the insertion of data into the relevant tables.

## Task 7: Average score

- Script: `7-average_score.sql`
- Description: Creates a stored procedure named `ComputeAverageScoreForUser` that computes and stores the average score for a student. The procedure takes `user_id` as an input and calculates the average score based on the data in the `corrections` table.

## Task 8: Optimize simple search

- Script: `8-index_my_names.sql`
- Description: Creates an index named `idx_name_first` on the `names` table, specifically on the first letter of the `name` column. This index improves the performance of searches based on the first letter of a name.

## Task 9: Optimize search and score

- Script: `9-index_name_score.sql`
- Description: Creates an index named `idx_name_first_score` on the `names` table, considering the first letter of the `name` column and the `score` column. This composite index further improves search performance by considering both name and score.

## Task 10: Safe divide

- Script: `10-div.sql`
- Description: Creates a function named `SafeDiv` that performs division, taking two arguments (`a` and `b`). The function returns the result of `a / b` if `b` is not zero; otherwise, it returns 0. It demonstrates error handling and safe division operations in SQL.

## Task 11: No table for a meeting

- Script: `11-need_meeting.sql`
- Description: Creates a view named `need_meeting` that lists all students who have a score below 80 and either no `last_meeting` date or a `last_meeting` date that is more than one month ago. This view helps identify students who require a meeting based on their scores and meeting history.

## Task 101: Average weighted score (Advanced)

- Script: `12-average_weighted_score.sql`
- Description: Creates a stored procedure named `ComputeAverageWeightedScoreForUser` that computes and stores the average weighted score for a student. The procedure considers the weights of projects and calculates the weighted average score based on the data in the `corrections` and `projects` tables.

Each script file can be executed on a MySQL database by using the command `mysql -uroot -p <filename>`. Make sure to replace `<filename>` with the actual name of the script file you want to execute.