# BBDD tarea 1 postgress

![image](https://user-images.githubusercontent.com/92529346/167946779-4869f2df-9027-43ed-832d-c3a01383e5ba.png)

Nos posicionamos en la carpeta 
___
![image](https://user-images.githubusercontent.com/92529346/167946829-774995fb-fb94-420f-b618-7c3b08e57eea.png)

![image](https://user-images.githubusercontent.com/92529346/167946920-7fca7b9d-5327-47eb-88d2-cf672c6ac117.png)

Ejecutamos el comando "code ." para abrir la carpeta en vscode o la abrimos con el editor de confianza, y creamos el archivo docker compose
___
![image](https://user-images.githubusercontent.com/92529346/167947014-bf861a5a-c490-434c-8b0a-07765f96f305.png)

Seguidamente usamos el comando "docker compose up -d" para crear el docker, indicando con el parametro -d que queremos tener el docker ejecutandose en segundo plano
___
![image](https://user-images.githubusercontent.com/92529346/167947083-30f6b148-9209-42cd-a9ab-5b0d84a985c2.png)

![image](https://user-images.githubusercontent.com/92529346/167947154-8b27059c-5e34-480d-b495-60967ec819eb.png)

A continuacion buscamos el nombre del docker con docker ps o lo comprobamos en el archivo docker-compose a preferencia, y ejecutamos el comando de la anterior imagen para abrir la terminal bash dentro del docker
___
![image](https://user-images.githubusercontent.com/92529346/167947695-05300c83-8dc5-4ea0-ab20-fee6ba421ad5.png)

![image](https://user-images.githubusercontent.com/92529346/167947834-c54f64d6-1a67-4d27-8e39-a3e2606e7d95.png)

![image](https://user-images.githubusercontent.com/92529346/167948330-ac0930c5-9223-4e5f-8e7f-396764351f4b.png)

Una vez dentro del docker creamos los usuarios y la base de datos con alumne0 como dueño, y para comprobar que todo haya funcionado correctamente podemos usar el comando psql para entrar en postgress y una vez dentro ejectuar el comando \l para listar las BBDD que tenemos
___
![image](https://user-images.githubusercontent.com/92529346/167948365-693d49a7-b745-40b3-8a5d-a16540501fa3.png)

Una vez este todo creado correctamente nos meteremos en la base de datos como alumne0 y crearemos una tabla e introduciremos datos
___
![image](https://user-images.githubusercontent.com/92529346/167948657-d9d2fc26-dec8-4f36-a9ac-434023922697.png)

Ahora comprobamos que como alumne no tenemos ningun permiso y no podemos hacer un SELECT de los datos
___
![image](https://user-images.githubusercontent.com/92529346/167948947-25eaf3dd-5167-49c0-9c63-9d12e35680ca.png)

![image](https://user-images.githubusercontent.com/92529346/167948960-0e4280d0-e2f2-42d7-830d-ea5c7082a941.png)

Volvemos a conectarnos como alumne0 y le damos permisos de SELECT a alune
___
![image](https://user-images.githubusercontent.com/92529346/167948966-324f0114-0dac-4e53-b834-87fd3a031a01.png)

Finalmente comprobamos que ahora podemos hacer un select de los datos que hay en la base de datos
___
