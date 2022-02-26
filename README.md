```sql
1. CREATE TABLE employee (
      id INTEGER PRIMARY KEY,
      name VARCHAR(50),
      birthdate DATE,
      email VARCHAR(100)
   );
```
```sql
2. INSERT INTO employee VALUES
      (1, 'Sheba', '12-11-1996', 'schitter0@cbc.ca'),
      (2, 'Olia', '28-02-1993', 'obusson1@bandcamp.com'),
      (3, 'Hartwell', '28-05-1978', 'hgolightly2@skyrock.com'),
      (4, 'Elysia', '19-04-1998', 'emattiacci3@ca.gov'),
      (5, 'Norbie', '15-09-1967', 'nwalder4@skype.com'),
      (6, 'Annaliese', '29-03-1981', 'aglynn5@youtu.be'),
      (7, 'Austina', '25-04-1997', 'apasticznyk6@chron.com'),
      (8, 'Edlin', '03-10-1978', 'ekarlik7@mediafire.com'),
      (9, 'Allistir', '14-07-1989', 'adurdan8@lulu.com'),
      (10, 'Selle', '18-08-1998', 'sbras9@admin.ch'),
      (11, 'Bret', '14-03-1975', 'bklawia@hhs.gov'),
      (12, 'Blanch', '17-12-1994', 'bardyb@dailymail.co.uk'),
      (13, 'Rosanne', '19-09-1978', 'rgeertsenc@github.com'),
      (14, 'Magdalena', '08-07-1986', 'mminified@topsy.com'),
      (15, 'Jecho', '27-09-1986', 'jolyfate@imageshack.us'),
      (16, 'Pietra', '01-04-1971', 'phaugheyf@hexun.com'),
      (17, 'Alfreda', '06-03-1999', 'asteelsg@disqus.com'),
      (18, 'Sorcha', '10-11-1978', 'slundbeckh@prweb.com'),
      (19, 'Deny', '11-07-1984', 'dhamshari@domainmarket.com'),
      (20, 'Saxon', '31-01-1964', 'scohalanj@paypal.com'),
      (21, 'Leontine', '23-09-1975', 'larnholdk@t-online.de'),
      (22, 'Rosamond', '14-06-1984', 'rginityl@ow.ly'),
      (23, 'Jilleen', '28-11-1979', 'jpullenm@bigcartel.com'),
      (24, 'Eva', '23-09-1993', 'echarltonn@geocities.com'),
      (25, 'Betti', '06-05-1998', 'bwinchursto@prnewswire.com'),
      (26, 'Ephrem', '04-11-1970', 'eangellp@fotki.com'),
      (27, 'Fair', '24-06-1987', 'fambrozq@nature.com'),
      (28, 'Jere', '16-06-1971', 'jtwaiter@digg.com'),
      (29, 'Jacquette', '20-02-1984', 'jtrans@unicef.org'),
      (30, 'Thorin', '02-11-1979', 'tmatiashvilit@shutterfly.com'),
      (31, 'Martha', '17-01-1982', 'mteazeu@blogspot.com'),
      (32, 'Ivie', '18-06-1972', 'isalmondv@npr.org'),
      (33, 'Gasper', '10-04-1989', 'ggaskw@storify.com'),
      (34, 'Allix', '05-06-1989', 'apipkinx@about.me'),
      (35, 'Heinrick', '23-06-1991', 'hstainlandy@cbc.ca'),
      (36, 'Melva', '22-04-1996', 'mbrindedz@photobucket.com'),
      (37, 'Anissa', '05-08-1980', 'afrankis10@springer.com'),
      (38, 'Rube', '25-01-1997', 'razam11@freewebs.com'),
      (39, 'Andrea', '24-10-1991', 'amerali12@toplist.cz'),
      (40, 'Nikita', '12-07-1978', 'npatrie13@wikimedia.org'),
      (41, 'Raviv', '06-04-1960', 'rgoodison14@stumbleupon.com'),
      (42, 'Shelli', '04-11-1996', 'sjeffree15@altervista.org'),
      (43, 'Cece', '18-08-1988', 'calejandro16@tinyurl.com'),
      (44, 'Jobye', '28-01-1985', 'jmarielle17@printfriendly.com'),
      (45, 'Coop', '23-05-1982', 'cpeel18@1688.com'),
      (46, 'Sheffield', '20-09-1974', 'slawrenz19@e-recht24.de'),
      (47, 'Christoph', '30-05-1988', 'chulle1a@people.com.cn'),
      (48, 'Sherline', '21-11-1978', 'snormanvill1b@printfriendly.com'),
      (49, 'Guglielma', '09-12-1975', 'gdeaconson1c@infoseek.co.jp'),
      (50, 'Brett', '06-07-1964', 'bkonrad1d@discovery.com');
```
```sql
3. UPDATE employee SET name = 'Ali' WHERE id = 1;
   UPDATE employee SET birthdate = '01-01-1990' WHERE name = 'Ali';
   UPDATE employee SET email = NULL WHERE birthdate > '01-01-1990';
   UPDATE employee SET birthdate = '01-01-2000' WHERE email IS NULL;
   UPDATE employee SET birthdate = NULL WHERE id % 2 = 1 AND id > 45;
```
```sql
4. DELETE FROM employee WHERE id = 50;
   DELETE FROM employee WHERE name LIKE 'Al%';
   DELETE FROM employee WHERE email IS NULL;
   DELETE FROM employee WHERE birthdate IS NULL;
   DELETE FROM employee WHERE ((DATE(NOW()) - DATE(birthdate)) / 365) < 25;
```
