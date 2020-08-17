## Express: Router Parameters

* Rather than always running middleware or manually adding middleware to specific routes, Express allows one to define parameters so that middleware is run only when those parameters are present and expected.

## Sub Documents in Mongoose

* Mongoose is a schema driven ORM that allows devs to add a layer of structure to the inherently unstructured NoSQL database model of MongoDB

[MongooseJS Documentation re: subdocuments](https://mongoosejs.com/docs/subdocs.html)

* **subdocuments** are documents embedded in other documents, meaning that you can nest schemas in other schemas (allowing for deeper levels of organization).

  - Subdocuments exist as arrays of subdocuments or single nested subdocuments
  - Subdocuments function like normal documents (can have middleware, custom validation logic, virtuals, etc) BUT they are not saved individually 

## Joining Data/Documents in Mongo

* populate() is a method that can be used on Mongoose to connect 2 collections in one of two ways:
  - by using a reference to another collection to physically join them
  - by using 'virtual population' to create a virtual field in a document that points to a field in another document OR by doing a collection 'on the fly' in pre('find')

---

[Home](https://jchinzi.github.io/reading-notes/)