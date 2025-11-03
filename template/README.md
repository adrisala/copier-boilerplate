# {{ project_name }}

{{ project_short_description }}

## Description

This is a Django REST Framework service created using the AAP Service Template.

## Features

- Django {{ django_version }}
- Django REST Framework
- Ready-to-use project structure
- Configured with development tools (black, flake8, isort, mypy)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/{{ author_name }}/{{ project_slug }}.git
cd {{ project_slug }}
```

2. Create and activate a virtual environment:
```bash
python{{ python_version }} -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -e ".[dev]"
```

4. Run migrations:
```bash
python manage.py migrate
```

5. Create a superuser:
```bash
python manage.py createsuperuser
```

6. Run the development server:
```bash
python manage.py runserver
```

## Development

### Running Tests
```bash
pytest
```

### Code Formatting
```bash
black .
isort .
```

### Linting
```bash
flake8
mypy .
```

## License

MIT

## Author

{{ author_name }}
