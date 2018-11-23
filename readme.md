1. Define CRUD.

    CRUD is create, read, update, and delete. This is a conceptual framework for working with web apps that use databases - each element of the SQL database needs to be able to utilize these functions

2. Why do we use set method_override: true?

    we employ the PUT method, which is not recognized by HTML, so using method_override allows us to pass it as a hidden value so that the controller can route the request correctly.

3. Explain the difference between value and name in this line: `<input type='text' name='task[title]' value="<%= @task.title %>"/>.`

    name is referencing a ruby hash to return something specific, and value is using an erb expression tag to create a template.

4. What are params? Where do they come from?

    Params appear to be a hash, but i think params is a class method that creates an instance of Parameters.new(value). They come from the ActionController::StrongParameters class.

5. Check out your routes. Why do we need two routes each for creating a new Task and editing an existing Task?

    The background processes required to edit or create are more complicated than the other methods because they involve manipulation of the SQL database in addition to the website's output.
