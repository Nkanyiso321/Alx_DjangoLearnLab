
---

### ✅ **3. update.md**

This file shows how you **change (update)** the Book’s title.

```markdown
# Update the Book title

```python
from bookshelf.models import Book

# Find the book
book = Book.objects.get(title='1984')

# Update the title
book.title = 'Nineteen Eighty-Four'
book.save()

# Check the updated book
print(book.title)

# Expected Output:
# Nineteen Eighty-Four
