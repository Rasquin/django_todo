# Install Django 1.11
sudo pip3 install django==1.11

# Create a Django project
django-admin startproject django_todo .

# Expose Django project at the ID and Port specified
python3 manage.py runserver $IP:$C9_PORT

# Add yourself to the allowed host list in  settings.py
ALLOWED_HOSTS = ['django-todo-rasquin.c9users.io']

# Add alias Shorcut to run your project
cog --> show home in favorites + hidden files --> workspace folder --> .bash_aliases folder
alias run="python3 ~/workspace/manage.py runserver $IP:$C9_PORT" 
the ~/workspace/manage.py is to ensure that no matter what directory we are in we have an absolute path to
manage.py file which will execute the command.

# Install Heroku
. Update npm, CLI
$ nvm i v8         # Any version > 8 will do e.g. nvm i v9 
. Install heroku cli
$ npm install -g heroku