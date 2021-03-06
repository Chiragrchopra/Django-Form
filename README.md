# Django-Form

An example of Django project with basic functionality.

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

## Screenshots

| Log In | Create an account | Authorized page |
| -------|--------------|-----------------|
| <img src="./screenshots/login.png" width="200"> | <img src="./screenshots/create_an_account.png" width="200"> | <img src="./screenshots/authorized_page.png" width="200"> |

| Password reset | Set new password | Password change |
| ---------------|------------------|-----------------|
| <img src="./screenshots/password_reset.png" width="200"> | <img src="./screenshots/set_new_password.png" width="200"> | <img src="./screenshots/password_change.png" width="200"> |


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
### Packages to be Installed on virtualenv

```
pip Django==2.1.9
pip django-bootstrap4==0.0.7
pip djangorestframework==3.9.4
pip pytz==2019.1

```
 or

```
pip install -r requirements.txt

```
### Configure the settings (connection to the database and SMTP server)

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
