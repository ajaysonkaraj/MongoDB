## Database commands

View all Database
```bash
  show dbs
```

Create or switch Database whose name is ajay
```bash
  use ajay
```
View current Database
```bash
  db
```
Delete the Database
```bash
  db.dropDatabase()
```

## Commands for Collections

Show Collections on the Database
```bash
  show collections
```
Create a Collection, name is student
```bash
  db.createCollection('student')
```
Delete the student collection
```bash
  db.student.drop()
```
