from bookshelf.models import Book

# Retrieve and delete the book
book = Book.objects.get(title="Nineteen Eighty-Four")
book.delete()

# Try to retrieve all books
books = Book.objects.all()
print(list(books))
# Output: []
