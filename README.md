# CURSO DE BOOTSTRAP
## INTRODUCCION
### ¿QUE ES UN FRAMEWORK FRONTEND?

Son una base para comenzar un proyecto permitiendo **flexibilidad en el diseño** 
Organizacion y estructura de nuestro HTML CSS y JavaScript
El componente principal es la grilla
Traen estilos para las fuentes
Además de componentes prearmados 


------------



### NUESTRO PROYECTO: HOLA MUNDO EN BOOTSTRAP

Vamos a sitio web oficial de Bootstrap en [Official Page](https://getbootstrap.com/ "Official Page") . Cualquier duda que tengas sobre los componentes y su uso que no se respondan en este curso, lo puedes encontrar en la sección de Documentation del sitio de Bootstrap.

Copiar el template de "starter template". Pegarlo en un archivo index.html. Abrir el archivo en el navegador


------------


[========]


## CREANDO EL SITIO WEB

### LA GRILLA DE BOOTSTRAP

- Dirigirise a la parte de `LAYOUT>GRIDS`
	- En esencia bootstrap tiene una grilla de 12 columnas

- Dirigirse a la parte de `LAYOUT > OPTIONS` 
	- En esa sección se verá los breakpoints los que bootstrap hace por defecto


------------

### EL FOOTER

HTML

       <footer id="footer" class="pb-4 pt-4"> <!-- padding bottom padding top -->
            <div class="container">
                <div class="row text-center">
                    <div class="col-12 col-lg">
                        <a href="#">Preguntas Frecuentes</a>
                    </div>
                    <div class="col-12 col-lg">
                        <a href="#">Contactanos</a>
                    </div>
                    <div class="col-12 col-lg">
                        <a href="#">Prensa</a>
                    </div>
                    <div class="col-12 col-lg">
                        <a href="#">Terminos y condiciones</a>
                    </div>
                </div>
            </div>
    
        </footer>

CSS

    #footer{
        background: linear-gradient(90deg, #1c3643, #273b47 25%, #1e5472);
    }
    
    #footer a {
        color: white;
        text-decoration: none;
    }
    
    #footer a:hover {
        text-decoration: underline;
    }


------------

### EL HEADER DE NUESTRO SITIO

[Bootstrap Navbar](https://getbootstrap.com/docs/5.0/components/navbar/ "Bootstrap Navbar")

    <nav class="navbar navbar-expand-lg navbar-light bg-light">
      <div class="container-fluid">
        <a class="navbar-brand" href="#">Navbar</a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav me-auto mb-2 mb-lg-0">
            <li class="nav-item">
              <a class="nav-link active" aria-current="page" href="#">Home</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Link</a>
            </li>
            <li class="nav-item dropdown">
              <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                Dropdown
              </a>
              <ul class="dropdown-menu" aria-labelledby="navbarDropdown">
                <li><a class="dropdown-item" href="#">Action</a></li>
                <li><a class="dropdown-item" href="#">Another action</a></li>
                <li><hr class="dropdown-divider"></li>
                <li><a class="dropdown-item" href="#">Something else here</a></li>
              </ul>
            </li>
            <li class="nav-item">
              <a class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true">Disabled</a>
            </li>
          </ul>
          <form class="d-flex">
            <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
            <button class="btn btn-outline-success" type="submit">Search</button>
          </form>
        </div>
      </div>
    </nav>
	


<img src="https://static.platzi.com/media/user_upload/header-4d3f241b-725d-435a-9a7e-ccdf6c5f7de3.jpg" alt="header y footer">

------------

### CREANDO UN CARROUSEL DE IMAGENES

[Carrusel Bootstrap](https://getbootstrap.com/docs/4.1/components/carousel/ "Carrusel Bootstrap")



------------

### AGREGANDO TEXTO INFORMATIVO DEL EVENTO

[Buttons Bootstrap](https://getbootstrap.com/docs/4.1/components/buttons/ "Buttons Bootstrap")

HTML



```
 <!-- agregando texto informatio del evento -->
              <div class="overlay">

                <div class="container">
                    <div class="row align-items-center">
                        <div class="col-md-6 offset-md-6 text-center text-md-end">
                            <h2>EUROFIGHTER GALLERY</h2>
                            <p class="d-none d-md-block">The world's most modern swing-role fighter</p>
                            <a href="#" class="btn btn-outline-light" data-toggle="modal">Ser parte</a>
                            <button type="button"  class="btn btn-platzi" data-toggle="modal" data-target="#modalCompra">Comprar</button>
                        </div>
                    </div>
                </div>

              </div>
```


CSS



```
/* agregando texto informativo del evento */

#carousel-fade {
    position: relative;
   
}

#carousel-fade .overlay {
    z-index: 1;
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    background-color: var(--carousel-bg-color);
    color: var(--just-white);
    
}

#carousel-fade .overlay .container,
#carousel-fade .overlay .row {
    height: 100%;
}
```

------------




------------



[========]