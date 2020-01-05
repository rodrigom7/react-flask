# react+flask

1. Crear el directorio flask-backend, los subdirectorios static y templates, y el archivo main.py.

2. instalar yarn

   - npm install -g yarn

3. instalar create-react-app y react-scripts

   - yarn global add create-react-app react-scripts

4. instalar flask

   - pip install flask

5. creamos la app de react y lo llamamos react-frontend

   - npx create-react-app react-frontend

6. Modificamos el main.py

7. nos movemos al directorio react-frontend y ejecutamos:

   - npm run eject

8. Vamos a la carpeta config y tenemos que modificar los archivos paths.js y webpack.config.js

   - En el primero modificamos appBuild: resolveApp('../flask-backend/static/react')
   - En el otro modificamos

     miniCssExtractPlugin:
     -filename: "css/[name].[contenthash:8].css"
     -chunckFilename: "css/[name].[contenthash:8].chunk.css"

     en htmlwebpackplugin, agregamos debajo de template:paths.appHtml
     -filename: "../../templates/index.html"

9. modificamos public/index.html en react-frontend

10. modificamos App.js

11. Agregamos en package.json debajo de -> "private": true
    - "homepage": "/static/react"
