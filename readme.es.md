# POSTERA

README en español [aqui](readme.es.md)

## Descripcion

Programa y publica en redes sociales los post obtenidos de varias redes sociales

- Soporte ES6 via [babel](https://babeljs.io)
- Recursos REST como middleware via [resource-router-middleware](https://github.com/developit/resource-router-middleware)
- Soporte CORS via [cors](https://github.com/troygoode/node-cors)
- Body Parsing via [body-parser](https://github.com/expressjs/body-parser)

> Tip: Si estas usando [Mongoose](https://github.com/Automattic/mongoose), puedes exponer automaticamente tus modelos como recursos REST usando [restful-mongoose](https://git.io/restful-mongoose).

## Empezando

```sh
# Clonalo
git clone git@github.com:developit/express-es6-rest-api.git
cd express-es6-rest-api

# Generate los archivos
rm -rf .git && git init && npm init

# Instala dependencias
npm install

# Inicia el desarrollo y servidor live-reload
PORT=8080 npm run dev

# Inicia el servidor de producción:
PORT=8080 npm start
```

## Soporte Docker

```sh
cd express-es6-rest-api

# Construye tu Docker
docker build -t es6/api-service.
#            ^      ^           ^
#          tag  tag name      Localización del Dockerfile

# ejecuta tu docker
docker run -p 8080:8080 es6/api-service
#                 ^            ^
#          bindea el puerto    container tag
#          a tu host
#          port de la maquina
```

## Licencia

[MIT](LICENCE)
