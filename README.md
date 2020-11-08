# Docker based LAMP

LAMP is abbreviate of Linux Apache MySQL/MariaDB PHP.

That mean complete environment for development on PHP language.

## How to use

Just copy docker-compose.yml from dist example

    cp docker-compose.dist.yml docker-compose.yml

Then build

    docker-compose build

And run composition

    docker-compose up -d

After this you may go to http://localhost and will see the default
index page.

Of course you wan to pass your PHP files to this composition, for this you
need overwrite strings like:

    - ./app:/var/www/html

To your path with sources, eg `- ../my-sources-in-parent-folder:/var/www/html`.