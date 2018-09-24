Questions
-- Return ALL the data in the 'movies' table.
```sql
SELECT * FROM movies;
```

-- Return ONLY the name column from the 'people' table
```sql
SELECT name FROM people;
```

-- Oops! Someone at CodeClan spelled Keith's name wrong! Change it to reflect the proper spelling.
```sql
UPDATE people
SET name = 'Keith Douglas'
WHERE id = 22;
SELECT name FROM people
```

-- Return ONLY your name from the 'people' table.
```sql
SELECT * FROM people
WHERE name = 'Iona Wright';
```

-- The cinema is showing 'Batman Begins', but Batman is DC, not Marvel! Delete the entry from the 'movies' table.
```sql
DELETE FROM movies
WHERE title = 'Batman Begins';
SELECT * FROM movies;
```

-- Create a new entry in the 'people' table with the name of one of the instructors.
```sql
INSERT INTO people (name) VALUES ('John Harper');
```

-- Pawel has decided to hijack our movie evening, Remove him from the table of people.
```sql
DELETE FROM people
WHERE name = 'Pawel'
```

-- The cinema has just heard that they will be holding an exclusive midnight showing of 'Avengers: Infinity War'!! Create a new entry in the 'movies' table to reflect this.
```sql
INSERT INTO movies (title, year, show_time) VALUES ('Avengers: Infinity War', 2018, '00:00');
```

-- The cinema would also like to make the Guardians movies a back to back feature. Find out the show time of "Guardians of the Galaxy" and set the show time of "Guardians of the Galaxy 2" to start two hours later.
```sql
SELECT * FROM movies
WHERE title LIKE '%Galaxy%';

UPDATE movies
SET show_time = '18:20'
WHERE id = 16;
SELECT * FROM movies

```
-- Delete multiple entries from your table in a single command.

```sql
DELETE FROM movies WHERE title LIKE '%Iro%';
```

-- Select all the movies ordered by year in descending order
```sql
SELECT * FROM movies
ORDER BY year DESC;
```


-------------------------------------------------------------------------------------------------------
