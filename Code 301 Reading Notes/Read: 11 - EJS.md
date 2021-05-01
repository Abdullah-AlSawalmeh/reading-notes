## EJS

- EJS is a simple templating language that lets you generate HTML markup with plain JavaScript.

1. Features

   - Fast compilation and rendering
   - Simple template tags: <% %>
   - Custom delimiters (e.g., use <? ?> instead of <% %>)
   - Includes
   - Both server JS and browser support
   - Static caching of intermediate JavaScript
   - Static caching of templates
   - Complies with the Express view system

2. set EJS as the view engine for our Express application using `app.set('view engine', 'ejs');`
3. send a view to the user by using `res.render()` (res.render() will look in a views folder for the view)
4. there will be a lot of code that is reused. We'll call those partials and define three files we'll use across all of our site: `head.ejs`, `header.ejs`, and `footer.ejs`.
5. Using Partials The syntax to use an EJS partial is: `<% include FILENAME %>`.
