
# PWA básica

----

> Ejemplo básico de una PWA. La app hace un **fetch** de un json y se almacena en un caché local

## Uso local

This demo app runs on `localhost`.

```bash
npm install http-server -g
http-server -c-1 # with cache disabled
```

Then open <http://localhost:8080> with Chrome.

Change `cacheStorageKey` in `sw.js` to update app version.

## Deploy automático

Al no requerir en este momento de un servidor, se usa [Netlify](app.netlify.com) para servir la aplicación en una URL pública (con https)

### Trouble shooting

* Why `-c-1` to disable cache?

`sw.js` can be cached by HTTP Caches, then in debugging we could get unexpected behaviors. Disable the cache to simplify the problem.

### License

MIT
