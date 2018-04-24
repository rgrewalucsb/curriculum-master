# Full-Stack Design Docs Preparation: Schema

The foundation of any of the apps you will be cloning is the information that it represents. Making sure that our tables and their corresponding ActiveRecord models have the correct columns, constraints, and associations is an integral part of understanding how our app should work.

Take some time to research the app you are cloning. While referring to your [MVPs][mvps] and making sure you're not going beyond the scope of this ten day full-stack project, try to break down and imagine the information you're seeing as tables. Keep in mind that some of the more abstract concepts, likes and follows for example, are usually represented by join tables.


[mvps]: ../../proposal/mvp-list.md

Create an outline of what your app's schema will look like. This should be an exhaustive set of table names, column names, and foreign key relationships for any of the resources your app will need to complete your MVP features.

# Bluebird Sample Schema





# Schema Information

## users
column name     | data type | details
----------------|-----------|-----------------------
id              | integer   | not null, primary key
username        | string    | not null, indexed, unique
password_digest | string    | not null
session_token   | string    | not null, indexed, unique

## chirps
column name | data type | details
------------|-----------|-----------------------
id          | integer   | not null, primary key
body        |  string   | not null
author_id   | integer   | not null, foreign key (references users), indexed
parent_chirp_id | integer | foreign key (references chirps), indexed

## hashtags
column name | data type | details
------------|-----------|-----------------------
id | integer | not null, primary key
slogan | string | not null

## hashtaggings
column name | data type | details
------------|-----------|-----------------------
id | integer | not null, primary key
chirp_id | integer | not null, foreign key (references chirps), indexed
hashtag_id | integer | not null, foreign key (references hashtags), indexed

## mentions
column name | data type | details
------------|-----------|-----------------------
id | integer | not null, primary key
user_id | integer | not null, foreign key (references users), indexed, part of a unique combination index with chirp_id
chirp_id | integer | not null, foreign key (references chirps), indexed, part of a unique combination index with user_id
