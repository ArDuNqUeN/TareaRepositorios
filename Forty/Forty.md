# Forty

[TOC]

## Trabajo en local

1. Inicializa un nuevo repositorio Git en una carpeta llamada "forty" y agrega los archivos proporcionados en el aula virtual. 

   ![image-20251020160429600](C:/Users/2dawv08/AppData/Roaming/Typora/typora-user-images/image-20251020160429600.png)

   ![image-20251020160452551](C:/Users/2dawv08/AppData/Roaming/Typora/typora-user-images/image-20251020160452551.png)

   ![image-20251020161339595](C:/Users/2dawv08/AppData/Roaming/Typora/typora-user-images/image-20251020161339595.png)

2. Renombra la rama master a main 

   ![image-20251020161415779](C:/Users/2dawv08/AppData/Roaming/Typora/typora-user-images/image-20251020161415779.png)

3. Haz que los ficheros README.txt , LICENSE.txt y passwords.txt sean ignorados por el control de versiones

   ![image-20251020161728811](C:/Users/2dawv08/AppData/Roaming/Typora/typora-user-images/image-20251020161728811.png)

   ![image-20251020162016337](C:/Users/2dawv08/AppData/Roaming/Typora/typora-user-images/image-20251020162016337.png)

4. Crea el archivo passwords.txt . Comprueba que el control de versiones lo ignora 

   ![image-20251020162308612](C:/Users/2dawv08/AppData/Roaming/Typora/typora-user-images/image-20251020162308612.png)

5. Crea una rama llamada "feature-content" . Muévete a esa rama. Cambia, en la línea 3477, el font-size por 1.5em en el archivo main.css . Confirma cambios y haz commit. Muestra los logs de la forma más gráfica posible. 

   ![image-20251020162828887](C:/Users/2dawv08/AppData/Roaming/Typora/typora-user-images/image-20251020162828887.png)

6. Elimina el archivo "passwords.txt" en la carpeta forty . Verifica el estado del repositorio. ¿Hay cambios pendientes?

   ![image-20251020163042741](C:/Users/2dawv08/AppData/Roaming/Typora/typora-user-images/image-20251020163042741.png)

7. Crea un nuevo archivo llamado " about.html ", partiendo del archivo generic.html y agrégalo al repositorio, haz un nuevo commit. 

   ![image-20251020163216002](C:/Users/2dawv08/AppData/Roaming/Typora/typora-user-images/image-20251020163216002.png)

8. Cambia a la rama main . Examina los logs del repositorio de forma gráfica. 

   ![image-20251020163318842](C:/Users/2dawv08/AppData/Roaming/Typora/typora-user-images/image-20251020163318842.png)

9. Modifica algo en el archivo generic.html , comprueba que hay cambios, y realiza otro commit . Examina los logs del repositorio de forma gráfica. 

   ![image-20251020163525201](C:/Users/2dawv08/AppData/Roaming/Typora/typora-user-images/image-20251020163525201.png)

10. Modifica algo en el fichero elements.html . Confirma los cambios, pero no hagas commit. 

    ![image-20251020163708488](C:/Users/2dawv08/AppData/Roaming/Typora/typora-user-images/image-20251020163708488.png)

11. Mira las diferencias de elements.html . Los cambios no nos gustan, deshaz los cambios de elements.html . Comprueba que no hay cambios pendientes. 

    ![image-20251020163810602](C:/Users/2dawv08/AppData/Roaming/Typora/typora-user-images/image-20251020163810602.png)

    se sale con "q"

    ![image-20251020164047486](C:/Users/2dawv08/AppData/Roaming/Typora/typora-user-images/image-20251020164047486.png)

12. Muestra las diferencias entre dos ramas. 

    ![image-20251020164209388](C:/Users/2dawv08/AppData/Roaming/Typora/typora-user-images/image-20251020164209388.png)

13. Fusiona la rama "feature-content" con la rama principal (main). Muestra los logs del repositorio de una forma gráfica y completa. 

    ![image-20251020164429141](C:/Users/2dawv08/AppData/Roaming/Typora/typora-user-images/image-20251020164429141.png)

    ![image-20251020164358502](C:/Users/2dawv08/AppData/Roaming/Typora/typora-user-images/image-20251020164358502.png)

14. Crea una nueva rama llamada " hotfix " y en ella, corrige un error crítico en el archivo " index.html ". (Por ejemplo, añade el enlace a la nueva página about.html) 

    ![image-20251020164848265](C:/Users/2dawv08/AppData/Roaming/Typora/typora-user-images/image-20251020164848265.png)

15. Fusiona la rama "hotfix" con la rama principal y verifica el historial de commits de forma que se vean todas las ramas gráficamente. ¿Borrarías la rama hotfix ? ¿En qué caso? ¿Cómo? 

    ![image-20251020164959178](C:/Users/2dawv08/AppData/Roaming/Typora/typora-user-images/image-20251020164959178.png)

    ![image-20251020165139582](C:/Users/2dawv08/AppData/Roaming/Typora/typora-user-images/image-20251020165139582.png)

    Intentaría tener siempre el número de ramas separado para cada archivo o grupos de archivos para evitar que los errores se expandan. pero una vez fusionadas no me sirven para nada.

16. Muestra el historial de cambios limitado a los últimos 3 commits. 

    ![image-20251020165215570](C:/Users/2dawv08/AppData/Roaming/Typora/typora-user-images/image-20251020165215570.png)

17. Etiqueta el commit actual como "v1.0" y muestra las etiquetas existentes.

    ![image-20251020165314873](C:/Users/2dawv08/AppData/Roaming/Typora/typora-user-images/image-20251020165314873.png)

## Trabajo en remoto

1. Sube al remoto los ficheros de tu repositorio local. Es necesario crear previamente en GitHub un repositorio llamado 'forty' NO crear archivo README.md en el remoto 

   ![image-20251023154754414](./Forty.assets/image-20251023154754414.png)

2. En local, crea una rama 'feature-head'. Cambia el título en la sección head de index.html , borra los comentarios del head , o previos, también. Confirma y sube los cambios al remoto.

   ![image-20251023154810759](./Forty.assets/image-20251023154810759.png)

3. En remoto, crea una rama 'feature-articulo'. Duplica la página generic , nómbrala como articulo.html , y añade como contenido un artículo sobre Git. Confirma los cambios y realiza un commit. Muestra los commits del repositorio tal como se ven en GitHub. 

   ![image-20251023154847586](./Forty.assets/image-20251023154847586.png)

   ![image-20251023155010486](./Forty.assets/image-20251023155010486.png)

   ![image-20251023155045088](./Forty.assets/image-20251023155045088.png)

   

4. En el repositorio local examina los cambios. Actualiza el repositorio con el remoto. Fusiona en 'main' las dos ramas 'feature'. Crea la etiqueta 'v2.0'. Muestra los logs, commits, etiquetas y ramas actuales, en local y en remoto 

   ![image-20251023155255082](./Forty.assets/image-20251023155255082.png)

   ![image-20251023155407733](./Forty.assets/image-20251023155407733.png)

5. En tu copia local, crea una rama nueva . En la rama nueva, cambia los enlaces de la página index.html para que apunten correctamente a la nueva página articulo.html . Confirma los cambios. 

   ![image-20251023155905596](./Forty.assets/image-20251023155905596.png)

6. Muestra los logs de forma que se vean las ramas en tu copia local. 

   ![image-20251023155939662](./Forty.assets/image-20251023155939662.png)

7. Te gusta el resultado de los cambios. Incorpora los cambios de la rama nueva a la principal.

   ![image-20251023160034594](./Forty.assets/image-20251023160034594.png)

8. Sube los cambios al remoto borrando la rama nueva , si es necesario. Comprueba primero con un comando en local, las ramas que hay en el repositorio remoto.

   ![image-20251023160309516](./Forty.assets/image-20251023160309516.png)

9. Muestra en local los cambios en el archivo index.html entre la versión actual y la anterior. 

   ![image-20251023160522194](./Forty.assets/image-20251023160522194.png)

10. En el repositorio en GitHub, navega hasta el archivo index.html y selecciona la opción "History".

    ![image-20251023160625978](./Forty.assets/image-20251023160625978.png)
