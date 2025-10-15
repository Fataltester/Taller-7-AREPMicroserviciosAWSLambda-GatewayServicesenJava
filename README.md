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

Parte II



