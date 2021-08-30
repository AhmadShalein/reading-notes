# Read 27: Django Models:

## Designing the LocalLibrary models

* The diagram shows the relationships between the models, including their multiplicities. The multiplicities are the numbers on the diagram showing the numbers (maximum and minimum) of each model that may be present in the relationship. For example, the connecting line between the boxes shows that Book and a Genre are related. The numbers close to the Genre model show that a book must have one or more Genres (as many as you like), while the numbers on the other end of the line next to the Book model show that a Genre can have zero or many associated books.

![LocalLibrary models](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Models/local_library_model_uml.svg)

* Model primer:

  * Models are usually defined in an application’s models.py file. They are implemented as subclasses of django.db.models.Model, and can include fields, methods and metadata.

* Fields:

  * A model can have an arbitrary number of fields, of any type — each one represents a column of data that we want to store in one of our database tables. Each database record (row) will consist of one of each field value.

* Methods:

  * A model can also have methods.

  * Minimally, in every model you should define the standard Python class method **str**() to return a human-readable string for each object.

----------------------------

## Django admin site

* The **Django admin application** can use your models to automatically build a site area that you can use to create, view, update, and delete records. This can save you a lot of time during development, making it very easy to test your models and get a feel for whether you have the right data. The admin application can also be useful for managing data in production, depending on the type of website.
