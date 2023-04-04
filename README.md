<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo_text.svg" width="320" alt="Nest Logo" /></a>
</p>

# Ejecutar en desarrollo

1. clonar el repositorio 
2. ejecutar
```
npm install
```
3. Tenete nest CLI install
```
npm i -g @nestjs/cli
```

4. Levantar la base de datos

```
docker-compose up -d
```
5. Clonar el archivo __.env.template__ y renombrar la copia a __.env__

6. LLenar las variables de entorno definidas en el __.env__

7. ejecutar la aplicacion en dev:
```
npm run start:dev
```

8. recontruir la db con seed

```
localhost:3000/api/v2/seed
```

## Stack usado

* MongoDB
* Nest js


# Production build

1. crear el archivo ```.env.pro```
2. llenar las variables de entorno de producción
3. crear la nueva imagen

```
docker-compose -f docker-compose.prod.yaml --env-file .env.prod up --build
```