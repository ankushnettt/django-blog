# Django Blog

A simple blogging web application built with **Django**. It provides the core structure for creating, storing, and displaying blog posts, complete with image upload support and a clean template-based front end.

> Repo: [ankushnettt/django-blog](https://github.com/ankushnettt/django-blog)

## Features

- 📝 Blog post creation and display via Django's app structure (`blog` app)
- 🖼️ Image uploads for posts (powered by Pillow, stored under `uploads/images`)
- 🎨 Custom static assets and HTML templates for the front end
- ⚙️ Standard Django project layout (`my_site`) for easy configuration and extension

## Tech Stack

| Component | Version |
|---|---|
| Python | 3.x |
| Django | 6.1 |
| Pillow | 12.3.0 |
| asgiref | 3.12.1 |
| sqlparse | 0.5.5 |

See [`requirements.txt`](requirements.txt) for the full list of dependencies.

## Project Structure

```
django-blog/
├── blog/                # Main blog app (models, views, urls, admin)
├── my_site/              # Django project settings and root URL config
├── static/                # CSS, JS, and other static assets
├── templates/             # HTML templates
├── uploads/images/        # User-uploaded post images
├── manage.py
└── requirements.txt
```

## Getting Started

### Prerequisites

- Python 3.10+ installed
- `pip` and (recommended) `virtualenv`

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/ankushnettt/django-blog.git
   cd django-blog
   ```

2. **Create and activate a virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Apply migrations**
   ```bash
   python manage.py migrate
   ```

5. **Create a superuser** (to access the Django admin)
   ```bash
   python manage.py createsuperuser
   ```

6. **Run the development server**
   ```bash
   python manage.py runserver
   ```

7. Open your browser at [http://127.0.0.1:8000/](http://127.0.0.1:8000/)

## Usage

- Visit `/admin/` and log in with your superuser credentials to create, edit, or delete blog posts.
- Uploaded images are saved to `uploads/images/` and served through Django's media handling.
- Customize templates in the `templates/` folder and styles in `static/` to change the look and feel.

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m "Add your feature"`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

## License

No license has been specified for this project yet. Consider adding a `LICENSE` file (e.g., MIT) to clarify how others can use your code.

## Author

**Ankush** — [@ankushnettt](https://github.com/ankushnettt)
