
---

### `retrieve.md`

```markdown
# Retrieve Operation

```python
# Retrieve the book we just created
book = Book.objects.get(title="1984")
print(book.title)
print(book.author)
print(book.publication_year)
