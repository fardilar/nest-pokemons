<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="120" alt="Nest Logo" /></a>
</p>

#Ejecutar en desarrollo

1. Clonar el repositorio 
2. Ejecutar 

```
npm install
```
3. Tener Nest cli instalado 
```
npm i -@nestjs/cli
```
4. Levantar la base de datos 
```
docker-composer up -d
```

5. Clonar Archivo __.env.template__ y renombrar a __.env__

6. Llenar las variables de entorno definias en el ```.env```

7. Ejecutar la aplicacion en modo dev
```
npm run start:dev
```

8. Reconstruir  la base de datos con la semilla 
```
http://127.0.0.1:3000/api/v2/seed
```


## Stack usado
* MongoDB
* Nest


## production build 
1. crear el archivo .env.prod
2. Llenar las variables de entorno 
3. Crear la imagen 
```
docker-compose -f docker-compose.prod.yaml --env-file .env.prod up --build
```