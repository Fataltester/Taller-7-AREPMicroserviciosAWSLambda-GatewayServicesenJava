# Hello World: AWS Lambda & Gateway Services en Java
## Juan David Martínez 
### Objetivo
Implementación de microservicios por medio de AWS lambda y AWS api gateway
### Parte 1 
1.Crear una clase que implemente el servicio deseado. Para esto usamos Java 21, Maven y Netbeans como IDE.

La clase MathServices fue creada como se solicitó y luego se generó el .jar
```bash
mvn package
```
2.Luego creamos la función lambda y cargamos las clases desarrolladas.

Accedemos al portal de AWS y buscamos "lambda".

Se crea la función lambda con java 21, subimos el .jar previamente generado y definimos como accedemos al método de la clase anteriormente creada

<img width="1609" height="707" alt="image" src="https://github.com/user-attachments/assets/3b17447c-1694-462e-ba70-bf65d1a27d2b" />

<img width="1655" height="194" alt="image" src="https://github.com/user-attachments/assets/1694db0c-e767-48b3-8b88-489691eb605e" />

Se realizó el siguiente test

<img width="1595" height="722" alt="image" src="https://github.com/user-attachments/assets/2e110f7f-8b62-433e-91cd-ce146014d699" />

<img width="1600" height="535" alt="image" src="https://github.com/user-attachments/assets/68541502-4525-4661-94c8-c19fb42fa97f" />


3.Luego configuramos el Gateway para exponer la función.

Accedemos al portal de AWS y buscamos "api gateway"

Siguiendo el tutorial creamos el api gateway, le asignamos unos métodos y submétodos, creamos el método relacionado a "square" de tipo GET y procedemos a configurar lo siguiente

* Method Request

<img width="1656" height="587" alt="image" src="https://github.com/user-attachments/assets/05063103-db3b-46e5-bbfe-e9a632d56311" />

* Integration Request

<img width="1688" height="785" alt="image" src="https://github.com/user-attachments/assets/98899aa4-1e1f-461b-abc3-0da9843a27eb" />

<img width="1369" height="404" alt="image" src="https://github.com/user-attachments/assets/f891d8ec-ac76-4be3-a199-08a380c858b9" />

Se realizó el siguiente test

<img width="1133" height="718" alt="image" src="https://github.com/user-attachments/assets/1b3d2da6-8f03-4bc1-be98-7a4af3d11837" />

Finalmente publicamos el API y accedemos a el mediante el browser

<img width="805" height="148" alt="image" src="https://github.com/user-attachments/assets/728f1f3d-7ed7-4df0-8f96-17c8dcf0fd6a" />

Parte II

Modificamos el código teniendo dos clases:

* SecurityUtils -> imprime el nombre y contraseña, setea la contraseña a vacío y retorna el usuario ya modificado.
* User -> contiene el nombre y la contraseña del usuario, con getters y setters

Teniendo ya las clases, nuevamente generamos el .jar para subirlo a una nueva función lambda
```bash
mvn package
```

Al igual que en el paso anterior, configuramos la función lambda con java 21 y definimos la ruta para acceder al método requerido

<img width="1597" height="702" alt="image" src="https://github.com/user-attachments/assets/ce65c566-a89e-4e46-8d83-51a18fd61269" />

<img width="1651" height="190" alt="image" src="https://github.com/user-attachments/assets/329003cb-47fb-4b61-a46c-4d73327f55fc" />

Se realizó el siguiente test

<img width="1595" height="720" alt="image" src="https://github.com/user-attachments/assets/6c613eb4-6467-4c74-b243-7bb2bfdf33f0" />

<img width="1593" height="713" alt="image" src="https://github.com/user-attachments/assets/2e96b25f-02e2-4b96-91e5-5b3dce11b06f" />

Luego nos vamos al mismo api gateway creado anteriormente para exponer el servicio, creamos el método para exponer el login y al igual que en la parte 1 modificamos lo siguiente

* Method Request

<img width="1643" height="632" alt="image" src="https://github.com/user-attachments/assets/e9d7ee10-efc8-4b83-8fc6-2c639ff8d0a9" />

* Integration Request

<img width="1619" height="718" alt="image" src="https://github.com/user-attachments/assets/43ba1354-1f00-4a09-bc2f-57b1b684ef8c" />

<img width="1332" height="476" alt="image" src="https://github.com/user-attachments/assets/81215774-0317-41db-b844-04fb3c114a61" />

Se realizó el siguiente test

<img width="1261" height="723" alt="image" src="https://github.com/user-attachments/assets/ae880898-0e16-4375-8ca8-273503b5fed3" />


Finalmente publicamos el API y accedemos a el mediante el browser

<img width="977" height="173" alt="image" src="https://github.com/user-attachments/assets/3c2b29fb-b821-47d6-9f0d-be088fc8f351" />




