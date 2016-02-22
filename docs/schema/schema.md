# Schema Information




## rooms
column name | data type | details
------------|-----------|-----------------------
id          | integer   | not null, primary key
title       | string    | not null
host_id     | integer   | not null, foreign key
type_id     | integer   | not null, foreign key
price       | float     | not null
location    | string    | not null
lat         | float     | not null
lng         | float     | not null

## room_galleries
column name | data type | details
------------|-----------|-----------------------
id          | integer   | not null, primary key
room_id     | integer   | not null, foreign key
photo_url   | string    | not null
result_photo| boolean   | not null
show_photo  | boolean   | not null
description | string    |

## reservation
column name | data type | details
------------|-----------|-----------------------
id          | integer   | not null, primary key
requester_id| integer   | not null, foreign key
room_id     | integer   | not null, foreign key
start_date  | date      | not null
end_date    | date      | not null
status      | string    | not null


## reviews
column name | data type | details
------------|-----------|-----------------------
id          | integer   | not null, primary key
rating      | integer   | not null
body        | text      | not null
reservation_id| integer | not null, foreign key

## user_profiles
column name | data type | details
------------|-----------|-----------------------
id          | integer   | not null, primary key
name        | string    | not null
user_id     | integer   | not null, foreign key
photo_url   | string    | not null
current_city| string    | not null

## users
column name     | data type | details
----------------|-----------|-----------------------
id              | integer   | not null, primary key
username        | string    | not null, indexed, unique
password_digest | string    | not null
session_token   | string    | not null, indexed, unique
