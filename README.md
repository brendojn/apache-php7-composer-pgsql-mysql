# apache-php7-composer-pgsql-mysql

This image has built in php7, apache, composer, php bindings for mysql and pgsql.

While running this, map the files you want to deploy to /var/www/html. For example, if your host side folder is ./app, use
```
docker run -v $(pwd)/app:/var/www/html .....
```

# Environment Variables
DOCUMENT_ROOT : If you don't specify this environment variable, /var/www/html is used by default.
API_TOKEN: If you specify a gitbub api token, this will help composer, so it won't ask for token during install.
