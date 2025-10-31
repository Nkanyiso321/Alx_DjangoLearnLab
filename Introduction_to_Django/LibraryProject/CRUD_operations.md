# CRUD Operations for Book Model

```python
from bookshelf.models import Book

# Create a Book instance
book = Book.objects.create(title='1984', author='George Orwell', publication_year=1949)
book
# Expected Output:
# <Book: 1984 by George Orwell (1949)>

# Retrieve all Book records
books = Book.objects.all()
for b in books:
    print(b.title, b.author, b.publication_year)
# Expected Output:
# 1984 George Orwell 1949

# Update the Book title
book = Book.objects.get(title='1984')
book.title = 'Nineteen Eighty-Four'
book.save()
updated_book = Book.objects.get(id=book.id)
print(updated_book.title)
# Expected Output:
# Nineteen Eighty-Four

# Delete the Book instance
book = Book.objects.get(title='Nineteen Eighty-Four')
book.delete()
Book.objects.all()
# Expected Output:
# <QuerySet []>
