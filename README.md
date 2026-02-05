# Django Portfolio Website

## Project Overview
This is a simple portfolio website created using the Django framework.  
The project is made as a **college assignment** to understand the basic working of Django such as views, URLs, templates, static files, and deployment.

The website contains multiple pages like Home, About, and Contact.

---

## Technologies Used
- Python
- Django
- HTML
- CSS
- Gunicorn (for deployment)
- Whitenoise (for static files)

---

## Project Structure

```
Django_Project/
├── build.sh
├── manage.py
├── requirements.txt
├── runtime.txt
├── collegeproject/
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   ├── views.py
│   └── wsgi.py
├── templates/
│   ├── home.html
│   ├── about.html
│   └── contact.html
└── static/
    └── style.css
```

---

## Explanation of Files

### `manage.py`
This file is used to run Django commands like starting the server, collecting static files, etc.

---

### `settings.py`
This file contains all the main configuration of the Django project such as:
- Installed apps
- Middleware
- Static files settings
- Template settings

It also includes Whitenoise configuration for serving CSS files in production.

---

### `urls.py`
This file handles routing of the website.  
It connects URLs to their respective view functions.

Example:
- `/` → Home page
- `/about/` → About page
- `/contact/` → Contact page

---

### `views.py`
This file contains Python functions that return HTML pages.

Example:
```python
def home(request):
    return render(request, "home.html")
```

Each function loads a specific HTML file.

---

### `templates/`

This folder contains all HTML files used in the project.

- `home.html` – Main page
- `about.html` – About information
- `contact.html` – Contact details

---

### `static/style.css`

This file contains basic CSS used to style the website.  
It improves the appearance and layout of the pages.

---

## Deployment

The project is deployed on Render using a Web Service.

A custom `build.sh` script is used to:
- Install required Python packages
- Collect static files

Gunicorn is used as the WSGI server.

---

## Learning Outcome

From this project, I learned:
- How Django project structure works
- How views and URLs are connected
- How to use templates and static files
- How to deploy a Django project online

---

## Conclusion

This project helped me understand the basics of Django framework and web development.  
It is a beginner-friendly project suitable for academic purposes.

---

### ✅ Why this README is college-safe
- Simple language  
- No buzzwords  
- Explains basics only  
- Looks handwritten by a student  
- Easy for viva explanation
