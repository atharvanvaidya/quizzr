# Quizzr

## An application to manage quizzes

## Why Quizzr?

Creating quiz questions is difficult, however storing, categorizing and conducting quizzes is way more difficult. 

Quiz masters generally use multiple tools like Powerpoint Presentation, Excel sheets, word documents to store and present quizzes.

Quizzr provides quiz master the features required to easily manage quizzes.

## Use Cases
* Should be platform agnostic.
* Ability to persist quiz data (Questions, as well as quiz rounds) on the machine
* Ability to export/import quiz data
* Supports these types of quizzes:
    - Infinite pounce : Question passes on in multiple rounds
    - Single pounce : Question passes on to each person only once.

## Tech Stack
* Python3
    - Flask
    - pytest

## Installation

### MySQL
Download [MySQL](https://dev.mysql.com/downloads/) and [MySQL Workbench](https://www.mysql.com/products/workbench/)

Create a new user using the following commands:
**NOTE**: Please change the below username and password
```sql
CREATE USER 'root1'@'localhost' IDENTIFIED BY 'zaq1ZAQ!';
```

Grant all access to the DB for this user : 
```sql
GRANT ALL PRIVILEGES ON *.* TO 'root1'@'localhost';
```

Reload to reflect the changes
```sql
FLUSH PRIVILEGES;
```