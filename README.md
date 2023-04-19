# django_social_media

Create and activate virtual environment:

```bash
conda create --name django_social_media --file requirements-env.txt django
```

If that doesn't work:

```bash
conda create --name django_social_media django
conda install -c conda-forge -n django_social_media misaka
```

Activate the virtual environment and add install the requirements:

```bash
activate django_social_media
pip install -r requirements.txt
```

Create and run migrations:

```bash
py manage.py migrate
py manage.py makemigrations accounts
py manage.py makemigrations groups
py manage.py makemigrations posts
py manage.py migrate
```

Run the server:

```bash
py manage.py runserver
```

Open [http://localhost:8000](http://localhost:8000) to view it in your browser.
