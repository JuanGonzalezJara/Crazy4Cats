Desafio Unidad 6 Modulo 3 (1)

#  Relaciones N a N en los modelos!

Desafio orientado a validar conocimientos de Relaciones N a N en los modelos. 

## Requerimientos

1. Set-up inicial del proyecto con sus relaciones y modelos.
2. La aplicación debe tener todas sus vistas bien estilizadas y con diseño agradable.
3. Implementar reacciones de un usuario a las publicaciones.
4. Implementar comentarios para las publicaciones.
5. Realizar deploy a Heroku con datos ficticios.


## Cuentas de prueba

Cuenta administrador:

- user: a@a.com
- password: 123456

Cuentas usuario:

- user: e@e.com
- password: 123456


```bash
En el archivo seed.rb podremos realizar la carga del siguiente set:

- 1 administrador
- 1 usuario
- 1 post

```




### Instalación 🔧

Clona el repositorio con el siguiente comando:

```bash
git clone https://github.com/JuanGonzalezJara/
```

En la terminal, accede a la carpeta donde se encuentra el repositorio y ejecuta (debes tener instalado Ruby y la gema bundle):

```bash
bundle install
```

Inicia la base de datos con el siguiente comando:

```bash
rails db:create db:migrate db:seed
```

Finalmente, ejecuta el proyecto con el siguiente comando y ve a la dirección IP que aparecerá en la consola:

```bash
rails s
```


## Subiendo proyecto a Heroku

- Deberas tener primero instalado Heroku en tu instancia de desarrollo, puedes realizarlo siguiendo el proceso desde la web de [heroku](https://id.heroku.com/login).
- Tambien deberas tener tu proyecto con Git inicializado o contar con la carpeta .git en tu proyecto

1: En la terminal, inicia sesión en Heroku:

```bash
heroku login
```

2: Crea una aplicación en Heroku:

```bash
heroku create
```

- Es importante copiar el nombre de la aplicación proporcionado por Heroku

3: Ahora conectaremos el proyecto con nuestra aplicación en Heroku:

```bash
heroku git:remote -a nombre-proyecto-dado_por_heroku
```

4: Realiza un push a Heroku:

```bash
git push heroku main
```

5: Debes ir a la página de tu aplicación en la web de [heroku](https://id.heroku.com/login) y dirigirte a la pestaña de la derecha que dice "More", Una vez que se despliegue el menú, selecciona la opción "Run console".

![Logo!](https://raw.githubusercontent.com/JuanGonzalezJara/TwitterClon/main/app/assets/images/heroku_menu_console.png?token=GHSAT0AAAAAACEFOVVZ3IZDU5RD6TGA7XBSZJHG6RA)


6: Una vez que se despliegue la consola, asegúrate de crear la base de datos si aún no está creada, migrar los cambios y generar los datos mediante el archivo seed.rb:

```bash
rails db:create
rails db:migrate
rails db:seed
```

Siguiendo estos pasos ya podras ver el funcionamiento de la aplicacion con los datos generados por el seed.


![Logo!](https://raw.githubusercontent.com/JuanGonzalezJara/Desafio_RoR_Unidad4_M3_3/main/assets/ROR_Logo.png)