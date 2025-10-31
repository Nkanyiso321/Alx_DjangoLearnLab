
---

### ✅ **2. retrieve.md**

This file shows how you **get (retrieve)** the Book you created.

```markdown
# Retrieve the created Book

```python
from bookshelf.models import Book

# Retrieve all books
books = Book.objects.all()
for b in books:
    print(b.title, b.author, b.publication_year)

# Expected Output:
# 1984 George Orwell 1949
