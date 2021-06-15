##Topic: Using illuminate Database With Eloquent in your PHP app without Laravel

In this tutorial, we will learn how to perform CRUD operations with the illuminate Database and Eloquent ORM by building the backend for a question and answer app.

The app will perform these tasks:
---------------------------------

* Add a user
* Add a question 
* Add an answer to a question 
* Upvote an answer 
* Get a question with answers 
* Get all questions and users who asked them 
* Get a particular questions answers and upvotes 
* Count questions by a particular user 
* Update answer by user
* Delete question 

Web with explain: https://code.tutsplus.com/tutorials/using-illuminate-database-with-eloquent-in-your-php-app-without-laravel--cms-27247?ec_unit=translation-info-language

Once you have cloned this repository, enter in the folder and run the commands:
  composer install
  composer dump-autoload -o

Questions
	
CREATE TABLE `questions` (
 `id` int(11) unsigned NOT NULL AUTO_INCREMENT,
 `question` tinytext,
 `user_id` int(11) DEFAULT NULL,
 `created_at` timestamp NULL DEFAULT NULL,
 `updated_at` timestamp NULL DEFAULT NULL,
 `deleted_at` timestamp NULL DEFAULT NULL,
 PRIMARY KEY (`id`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8;
