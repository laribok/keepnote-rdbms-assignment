## Table Creations
```
CREATE TABLE notemanagement.user (
    user_id INT,
    user_name VARCHAR(255),
    user_added_date DATE,
    user_password VARCHAR(255),
    user_mobile VARCHAR(10)
)
```

```
CREATE TABLE notemanagement.note (
    note_id INT,
    note_title VARCHAR(255),
    note_content VARCHAR(1024),
    note_status VARCHAR(255),
    note_creation_date DATE
)
```

```
CREATE TABLE notemanagement.category (
    category_id INT,
    category_name VARCHAR(255),
    category_descr VARCHAR(512),
    category_creation_date DATE,
    category_creator VARCHAR(512)
)
```

```
CREATE TABLE notemanagement.reminder (
    reminder_id INT,
    reminder_name VARCHAR(255),
    reminder_descr VARCHAR(255),
    reminder_type VARCHAR(255),
    reminder_creation_date DATE,
    reminder_creator VARCHAR(255)
)
```

```
CREATE TABLE notemanagement.notecategory (
    notecategory_id INT,
    note_id INT,
    category_id INT
)
```

```
CREATE TABLE notemanagement.notereminder (
    notereminder_id INT,
    note_id INT,
    reminder_id INT
)
```

```
CREATE TABLE notemanagement.usernote (
    usernote_id INT,
    user_id INT,
    note_id INT
)
```