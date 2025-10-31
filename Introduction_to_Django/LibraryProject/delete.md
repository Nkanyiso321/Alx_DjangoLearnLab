
---

### `delete.md`

```markdown
# Delete Operation

```python
# Delete the book
book = Book.objects.get(title="Nineteen Eighty-Four")
book.delete()

# Confirm deletion
books = Book.objects.all()
print(books)
