## React WordPress Theme

## Development Guide
- **`docker-compose up -d`** - start mysql and wordpress containers and start using your application at [127.0.0.1:8000](http://127.0.0.1:8000).
- **`docker-compose down`** - stop the application. Pass `-v` to destroy mysql volume.
- **`docker-compose up -d --build`** - rebuilds the WordPress image (eg. because you changed something in the sources).
- **` gulp`** - Will compile, start BrowserSync and watch for any changes.
- **`gulp production`** - Will compile and minify assets.

## Built using
- Wordpress
- Docker
- React

Forked from **[WordPress starter theme with React.js integrated](https://github.com/itzikbenh/WReact)**
