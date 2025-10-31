
---

### ✅ **4. delete.md**

This file shows how you **delete** the Book.

```markdown
# Delete the Book instance

```python
from bookshelf.models import Book

# Find the book
book = Book.objects.get(title='Nineteen Eighty-Four')

# Delete it
book.delete()

# Confirm deletion
Book.objects.all()

# Expected Output:
# <QuerySet []>
