## Design for a Hello World Website using Flask and Bootstrap

### HTML Files

- **index.html**

This is the main page of the website. It contains the HTML5 code for the home page of the website. It should include a basic HTML structure, such as the head and body elements, as well as the necessary Bootstrap elements to create the layout of the home page.

```html
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/css/bootstrap.min.css" rel="stylesheet" />
  <title>Hello World</title>
</head>

<body>
  <div class="container">
    <h1>Hello World!</h1>
    <p>This is a hello world website made with Flask and Bootstrap.</p>
  </div>
</body>

</html>
```

### Routes

- **@app.route('/')**

This route is used to map the URL '/' to the index.html page. When a user visits the root URL of the website (e.g., https://example.com/), this route will serve the index.html page, which will display the home page of the website.

```python
@app.route('/')
def index():
  return render_template('index.html')
```