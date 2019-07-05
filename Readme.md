

## Pasos para correr la aplicación (API)
1. **Clonar la aplicación**

	```bash
	git clone https://github.com/callicoder/spring-security-react-ant-design-polls-app.git
	cd polling-app-server
	```

2. **Crear la Base de Datos**

	```bash
	create database polling_app
	```

3. **Configurar el  los parámetros locales de tu base de datos MySQL**

	+ abre el archivo `src/main/resources/application.properties` .

	+ cambia las propiedades `spring.datasource.username` y `spring.datasource.password` para que concuerden con tu instalación local

4. **Correr la aplicación**

	Para correr la app (servidor) corre el siguiente comando -

	```bash
	mvn spring-boot:run
	```

	el servidor iniciará en el puerto 8080.

	Puedes empaquetar la aplicación en forma de archivo `jar` y luego corriendo haciendo lo siguiente -

	```bash
	mvn package
	java -jar target/polls-0.0.1-SNAPSHOT.jar
	```

## Pasos para correr la App React (página web)

Primero ve a la carpeta `polling-app-client` folder -

```bash
cd polling-app-client
```

Luego escribes los siguientes comandos para iniciar la página web  -

```bash
npm install && npm start
```

El servidor front-end iniciará en el puerto `3000`.
