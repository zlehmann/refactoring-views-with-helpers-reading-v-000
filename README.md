## Objectives

1. Understand when to use Helper methods
2. Create Helper methods for specific controllers
3. Create application wide helpers

## Outline

Taking them through the flow of discovery for learning about controller specific actions and then to application helpers. To have them follow along, include [this](https://github.com/learn-co-curriculum/activerecord-lifecycle-reading) rails app. Simple blog with authors/posts

  * Imagine we have a blog with posts. Posts have an `updated_at` field.
  * Write it in the `show` the code to `strftime` the `updated_at`
  * Write the same code in the `index`
  * Then write the same code in the `_form` for `edit`. (Last updated: BLAH)
  * Code Repetition!
    * Belong in the model? No this has nothing to do with the DB
    * This only has to do with presentation layer stuff
    * So create a helper in the blog helpers
  * Our blog also has an Author
  * When you go to the author show page, it also wants to show the updated date
    * We can access any controllers helpers so we can use the blog one
    * Remember we want devs to be able to guess where code lives. Does date stuff belong in blog?
    * nope. put it in applicationcontroller
  
