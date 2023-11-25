```markdown
# TweakedDB

TweakedDB is a lightweight file-based database library for Python with 64-bit encryption. It provides a simple key-value store with basic CRUD operations.


```

## Installation

```bash
pip install tweaked
```

## Quick Start

```python
from tweaked import TweakedDB

# Initialize the database with a filename and a secret key
db = TweakedDB('mydatabase.tw', 'mysecretkey')

# Set values
db.set('name', 'John Doe')
db.set('age', '30')

# Get values
name = db.get('name')
print(f"Name: {name}")

# Delete a key
db.delete('age')

# Get all keys
all_keys = db.get_all_keys()
print(f"All Keys: {all_keys}")
```

## Methods

### `set(key, value)`

Sets the value for a given key in the database.

### `get(key)`

Retrieves the value for a given key from the database.

### `delete(key)`

Deletes a key-value pair from the database.

### `get_all_keys()`

Returns a list of all keys in the database.

## File Format

Data is stored in a text file with each key-value pair on a new line. Keys and values are separated by a colon.

## Encryption

TweakedDB uses 64-bit encryption to secure the data. The encryption key is derived from the secret key provided during initialization.

## Contributing

If you'd like to contribute to TweakedDB, please fork the repository, make your changes, and submit a pull request.

## Maintainers

TweakedDB is maintained by Cities and Sizzor. If you encounter any issues or have questions, you can contact them on Discord:

- Cities: `mlg0001` (Discord Tag)
- Sizzor: `.sizzor` (Discord Tag)


