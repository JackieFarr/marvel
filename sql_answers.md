Questions

```sql

<!-- Return ALL the data in the 'movies' table. -->
SELECT * FROM movies;

<!-- Return ONLY the name column from the 'people' table -->
SELECT name FROM people;

<!-- Oops! Someone at CodeClan spelled Keith's name wrong! Change it to reflect the proper spelling. -->
UPDATE people
SET name = 'Keith Douglas'
WHERE id = 22;

<!-- Return ONLY your name from the 'people' table. -->
SELECT name FROM people WHERE name = 'Jackie Farr';

<!-- The cinema is showing 'Batman Begins', but Batman is DC, not Marvel! Delete the entry from the 'movies' table. -->
DELETE FROM movies
WHERE title = 'Batman Begins';

-- Create a new entry in the 'people' table with the name of one of the instructors.
INSERT INTO people (name) VALUES ('John Harper');

-- Pawel has decided to hijack our movie evening, Remove him from the table of people.
??????????????????????????

-- The cinema has just heard that they will be holding an exclusive midnight showing of 'Avengers: Infinity War'!! Create a new entry in the 'movies' table to reflect this.
INSERT INTO movies (title, year, show_time) VALUES ('Avengers: Infinity War', 2018, '00:00');

-- The cinema would also like to make the Guardians movies a back to back feature. Find out the show time of "Guardians of the Galaxy" and set the show time of "Guardians of the Galaxy 2" to start two hours later.
UPDATE movies
SET show_time = '18.40'
WHERE title = 'Guardians of the Galaxy 2';

Extension

-- Delete multiple entries from your table in a single command.
DELETE FROM movies
WHERE title LIKE '%Iron%';

-- Select all the movies ordered by year in descending order
SELECT * FROM movies ORDER BY year DESC;

```
