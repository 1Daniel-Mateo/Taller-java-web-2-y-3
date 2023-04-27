##BIENVENIDOS AL REPOSITORIO DEL TALLER 2 DE JAVA AVANZADO

**Descripción**
En talller se enfoco en crear dos paginas web una de login y otra de registro usuario, tambien se trabajo el desarrollo de enlazarla con una bases de datos de usuarios basica.

**Requisitos para su desarrollo**

*1. Tener instalado el editor de programación iintellij idea con la licencia.*
*2. Crear las respectivas carpetas que el instrutor recomendo durante el proceso formación.*
*3. Entender como se enlazan la base de datos, aun que en este caso la conexion se trabajara otras clases.*

**Funcionamiento**

*El proyecto la carpeta src en el cual esta el index donde haremos el login y la carpeta jsp donde guardaremos el register*

    <!DOCTYPE html>
    <html lang="es">
    <head>
     <meta charset="utf-8">
        <meta name="author" content="Mateo Suarez">
        <meta name="description" content="Regitro de usuario y logeo de usuario">
        <meta name="keywords" content="registro de usuario, formulario de registro, crear cuenta, registro en linea">
        <meta name="viewport" content="width=device-width, initial-scale=1">
        <title>LOGEO DE USUARIO : MY APP</title>
        <link rel="icon" type="image/x-icon" href="../img/barateon.png">
        <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-KK94CHFLLe+nY2dmCWGMq91rCGa5gtU4mk92HdvYe+M/SXH301p5ILy+dN9+nJOZ" crossorigin="anonymous">
        <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icon@1.10.3/font/bootstrap-icons.css">
        <link rel="stylesheet" href="../css/signin.css">
        <link rel="stylesheet" href="../css/styles.css">
    </head>
    <body>
<header>
    </header>
    <nav>
    </nav>
<section>
</section>
<footer>
</footer>
    </body>
    </html>

*enlaces para los estilos con css ademas del bootstrap y la carpeta img para el logo e icono*


    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-KK94CHFLLe+nY2dmCWGMq91rCGa5gtU4mk92HdvYe+M/SXH301p5ILy+dN9+nJOZ" crossorigin="anonymous">
        <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icon@1.10.3/font/bootstrap-icons.css">
        <link rel="stylesheet" href="../css/signin.css">
        <link rel="stylesheet" href="../css/styles.css">
    
    <img src="../img/barateon.png" class="mb-4" alt="MY APP" width="100">
*Una base de datos sql de la tabla usuarios*
```java
package com.example.project2687365.models;

public class User {
    private Integer user_id;
    private String user_firstname;

    private String user_lastname;
    private String user_email;
    private String user_password;

    public User(){

    }

    public User(Integer user_id, String user_firstname, String user_lastname, String user_email, String user_password) {
        this.user_id = user_id;
        this.user_firstname = user_firstname;
        this.user_lastname = user_lastname;
        this.user_email = user_email;
        this.user_password = user_password;
    }

    public Integer getUser_id() {
        return user_id;
    }

    public void setUser_id(Integer user_id) {
        this.user_id = user_id;
    }

    public String getUser_firstname() {
        return user_firstname;
    }

    public void setUser_firstname(String user_firstname) {
        this.user_firstname = user_firstname;
    }

    public String getUser_lastname() {
        return user_lastname;
    }

    public void setUser_lastname(String user_lastname) {
        this.user_lastname = user_lastname;
    }

    public String getUser_email() {
        return user_email;
    }

    public void setUser_email(String user_email) {
        this.user_email = user_email;
    }

    public String getUser_password() {
        return user_password;
    }

    public void setUser_password(String user_password) {
        this.user_password = user_password;
    }

    @Override
    public String toString() {
        return "User{" +
                "user_id=" + user_id +
                ", user_firstname='" + user_firstname + '\'' +
                ", user_lastname='" + user_lastname + '\'' +
                ", user_email='" + user_email + '\'' +
                ", user_password='" + user_password + '\'' +
                '}';
    }