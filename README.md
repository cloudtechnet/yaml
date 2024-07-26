YAML (YAML Ain't Markup Language) is a human-readable data serialization standard that is commonly used for configuration files and data exchange between languages with different data structures. It's designed to be easy to read and write, which makes it ideal for configuration files, data storage, and transmission.


### 1. **Key-Value Pairs**
![Key-Value Pairs](https://via.placeholder.com/15/0000FF/000000?text=+) **Key-Value Pairs**
YAML uses simple key-value pairs to represent data.

```yaml
name: Rajesh
age: 35
```

### 2. **Nested Structures**
![Nested Structures](https://via.placeholder.com/15/FF0000/000000?text=+) **Nested Structures**
YAML supports nested data structures, using indentation to denote hierarchy.

```yaml
address:
  street: 123 Main St
  city: Hyderabad
  state: Telangana
```

### 3. **Lists**
![Lists](https://via.placeholder.com/15/00FF00/000000?text=+) **Lists**
YAML uses hyphens (`-`) to represent items in a list.

```yaml
languages:
  - Python
  - Java
  - YAML
```

### 4. **Comments**
![Comments](https://via.placeholder.com/15/808080/000000?text=+) **Comments**
YAML supports comments, which start with the `#` symbol.

```yaml
# This is a comment
name: Rajesh  # This is an inline comment
```

### 5. **Multiline Strings**
![Multiline Strings](https://via.placeholder.com/15/FFA500/000000?text=+) **Multiline Strings**
YAML allows multiline strings using `|` for literal blocks or `>` for folded blocks.

```yaml
description: |
  This is a multiline string.
  It can contain newlines and indentation.
```

```yaml
summary: >
  This is a folded multiline string.
  Newlines become spaces.
```

### 6. **Dictionaries**
![Dictionaries](https://via.placeholder.com/15/8A2BE2/000000?text=+) **Dictionaries**
Dictionaries (or maps) can be represented inline using curly braces or in a block style.

```yaml
inline_dictionary: { key1: value1, key2: value2 }

block_dictionary:
  key1: value1
  key2: value2
```

### 7. **Anchors and Aliases**
![Anchors and Aliases](https://via.placeholder.com/15/DC143C/000000?text=+) **Anchors and Aliases**
YAML supports anchors (`&`) and aliases (`*`) to reuse data.

```yaml
defaults: &defaults
  adapter: postgres
  host: localhost

development:
  database: dev_db
  <<: *defaults  # Merge defaults
```

### 8. **Boolean Values**
![Boolean Values](https://via.placeholder.com/15/FFD700/000000?text=+) **Boolean Values**
YAML represents boolean values with `true` and `false`.

```yaml
is_active: true
is_admin: false
```

### 9. **Null Values**
![Null Values](https://via.placeholder.com/15/ADFF2F/000000?text=+) **Null Values**
Null values in YAML are represented with `null` or `~`.

```yaml
middle_name: null
nickname: ~
```

### 10. **Numbers**
![Numbers](https://via.placeholder.com/15/00CED1/000000?text=+) **Numbers**
YAML supports integers and floating-point numbers.

```yaml
age: 35
height: 5.9
```

### 11. **Special Characters**
![Special Characters](https://via.placeholder.com/15/FF69B4/000000?text=+) **Special Characters**
YAML allows special characters using escape sequences.

```yaml
special: "This is a string with a newline\ncharacter."
```
