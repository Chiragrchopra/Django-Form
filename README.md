# Django-Form

An example of Django project with basic functionality.

## Screenshots

| Log In | Create an account | Authorized page |
| -------|--------------|-----------------|

| Password reset | Set new password | Password change |
| ---------------|------------------|-----------------|

## Functionality

- Log in
    - via username & password
    - via email & password
    - via email or username & password
    - with a remember me checkbox (optional)
- Create an account
- Log out
- Profile activation via email
- Reset password
- Remind a username
- Resend an activation code
- Change password
- Change email
- Change profile
- Multilingual: English, Russian, and Simplified Chinese


## Installing

### Clone the project

```
git clone https://github.com/Chiragrchopra/Django-Form
cd Django-Form
```

### Install dependencies & activate virtualenv

```
pip install pipenv

pipenv install
pipenv shell
```
### packages to be Installed on virtualenv

certifi==2019.6.16
Django==2.1.9
django-bootstrap4==0.0.7
djangorestframework==3.9.4
pipenv==2018.11.26
pytz==2019.1

### Configure the settings (connection to the database, connection to an SMTP server, and other options)

1. Edit `source/app/conf/development/settings.py` (For development)

2. Edit `source/app/conf/production/settings.py` (For production)

### Apply migrations

```
python source/manage.py migrate
```

### Collect static files (only on a production server)

```
python source/manage.py collectstatic
```

### Running

#### A development server

Just run this command:

```
python source/manage.py runserver
```
