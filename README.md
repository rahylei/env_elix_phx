# env_elix_phx
Ambiente de desarrollo para trabajar con elixir y phoenix framework

# comandos
1. **docker  compose up -d**
  - *Cuando se crea esto, se genera una imagen con el nombre de esta carpeta, esta va a ser usada para correr el segundo comando.*
2. **docker run -it --rm -u "$(id -u):$(id -g)" --network test_template_default -p4000:4000 -v $(pwd):/app -w /app nombre-carpeta-app bash**
  - *Ya con este estamos dentro de la teminar del projecto y podemos usar tanto mix como iex.*
  
# Prepaciones

Cuando se generen projectos hay que que modificar los valores de configuracion que apuntan a localhost asi como el nombre del host de la base de datos. 
Para el primero tiene cambiar el local host **127.0.0.1** por *0.0.0.0*, y en el nombre del host de la base de datos colocar **"database"**.

*En el case de los test es necario tambien cambiar la direcion a la que apunta el host de la base de datos para evitar errores.*
