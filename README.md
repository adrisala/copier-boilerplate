# Django REST Framework Copier Template

This is a Copier template for creating Django REST Framework projects. It was converted from a Cookiecutter template.

## Prerequisites

- Python 3.10 or higher
- [Copier](https://copier.readthedocs.io/) installed (`pip install copier`)

## Usage

To create a new project from this template:

```bash
copier copy path/to/copier-boilerplate /path/to/your/new/project
```

Or if using a git repository:

```bash
copier copy gh:yourusername/copier-boilerplate /path/to/your/new/project
```

You will be prompted to answer the following questions:

- **project_name**: The human-readable name of your project (default: "My Django Project")
- **project_slug**: The slug used for directory and module names (auto-generated from project_name)
- **project_short_description**: A brief description of your project
- **author_name**: Your name or organization name
- **version**: Initial version number (default: "0.1.0")
- **python_version**: Python version to use (choices: 3.10, 3.11, 3.12)
- **django_version**: Django version (default: "5.2")

## Updating an Existing Project

To update a project that was created with this template:

```bash
cd /path/to/your/project
copier update
```

This will apply any changes from the template to your project.

## Template Features

The generated project includes:

- Django 5.2+
- Django REST Framework
- Pre-configured development tools:
  - pytest for testing
  - black for code formatting
  - flake8 for linting
  - isort for import sorting
  - mypy for type checking
- Ready-to-use project structure
- Configuration files (pyproject.toml)
- Example app (`main`)

## Template Structure

```
copier-boilerplate/
├── copier.yml                  # Copier configuration
├── README.md                   # This file
└── template/                   # Template files
    ├── .copier-answers.yml.jinja
    ├── .gitignore
    ├── README.md
    ├── pyproject.toml
    ├── requirements.txt
    ├── manage.py
    ├── {{ project_slug }}/     # Main project directory
    │   ├── __init__.py
    │   ├── asgi.py
    │   ├── settings.py
    │   ├── urls.py
    │   └── wsgi.py
    └── main/                   # Example app
        ├── __init__.py
        ├── admin.py
        ├── apps.py
        ├── models.py
        ├── settings.py
        ├── tests.py
        ├── urls.py
        └── views.py
```

## Differences from Cookiecutter

This template has been converted from Cookiecutter to Copier. Key differences:

1. **Configuration file**: `copier.yml` instead of `cookiecutter.json`
2. **Template syntax**: Jinja2 `{{ variable }}` instead of `{{cookiecutter.variable}}`
3. **Template directory**: Files are in `template/` subdirectory
4. **Template suffix**: `.jinja` suffix for template files (configured as `_templates_suffix`)
5. **Update support**: Copier natively supports updating existing projects

## License

MIT
