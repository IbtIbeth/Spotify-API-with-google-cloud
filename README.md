# Spotify-API-with-google-cloud

Análisis simple usando Google Cloud




Depósitos de datos 


Ibeth Escobedo Rios
Luis David Huante

Profesor: Héctor Alonso Guzmán Gutiérrez





## Obtención de datos

Con la API de spotify se obtuvo diferentes tipos de datos, en primer lugar la información de los 10 artistas más escuchados a través de toda la historia en dicha plataforma, en segundo lugar se obtuvo los últimos 20 álbumes de dichos artistas.

Los artistas más escuchados son: 

Taylor Swift


Justin Bieber


BTS


Drake


Bad Bunny


Rihanna


Ariana Grande


Ed Sheeran


Billie Eilish


Eminem



(No están ordenados )

Con estos datos se crearon dos tablas artista y album_artistas. El diagrama lógico relacional quedó de esta manera: 














Los registros que se le insertaron a la tabla artista fueron:



Algunos de los registros insertados a la tabla album_artistas fueron: 



Estos datos se subieron a sus respectivas tablas a google cloud con ayuda de mySQL y python, el código se encuentra en el siguiente repositorio: https://github.com/IbtIbeth/Spotify-API-with-google-cloud

Lo siguiente es crear una instancia con su respectiva base de datos, teniendo una IP pública y en el código que se llenaran los datos como el usuario, ip, host y base de datos.

Una vez teniendo todo lo anterior es momento de hacer una big query en google cloud. En este caso haremos una consulta uniendo las dos tablas y lo que queremos es: “Mostrar los nombres de los álbumes, el número de canciones y el artista que interpreta dicho álbum donde en el álbum contenga más de 20 canciones”


