# Delete Operation

```python
book = Book.objects.get(title='Nineteen Eighty-Four')
book.delete()
Book.objects.all()
```

# Expected Output:
<QuerySet []> (Empty — book deleted successfully)
