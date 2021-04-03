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

### AGREGANDO BOTONES

[Botones](https://getbootstrap.com/docs/4.1/components/buttons/ "Botones")

HTML


```
 <button type="button"  class="btn btn-brand" data-toggle="modal" data-target="#modalCompra">Comprar</button>
```



CSS



```
.btn-brand {
    background-color: var(--main-color-brand);
    color: var(--just-white);
}

.btn-brand:hover {
    background-color: var(--second-color-brand);
}

```



------------

### LAS CARDS DE BOOTSTRAP

[CARDS](https://getbootstrap.com/docs/5.0/components/card/ "CARDS")

HTML

  <!-- SPEAKERS -->

    <section id="speakers" class="mt-4 mb-4"><!-- mt=margin-top -->
        <div class="container row">
            <div class="col text-center text-uppercase">
                <small>Conoce a los </small>
                <h2>Oradores</h2>
            </div>
        </div>
        <!-- HERE COMES THE CARDS -->
        <div class="row">
            <div class="col-12 col-md-6 col-lg-4 mb-4">
                <div class="card" style="width: 18rem;">
                    <img src="./assets/img/mig1.jpg" class="card-img-top" alt="...">
                    <div class="card-body">
                      <h5 class="card-title">Air superiority</h5>
                      <p class="card-text">In the air superiority mission the Eurofighter Typhoon will typically be equipped with air-to-air missiles for the BVR and short range combat. It is the combination of thrust, maneuverability, modern sensors and data fusion that makes the Eurofighter Typhoon the superior air warfare platform.</p>
                      
                    </div>
                </div>
            </div>
            <div class="col-12 col-md-6 col-lg-4 mb-4">
                <div class="card" style="width: 18rem;">
                    <img src="./assets/img/mig2.jpg" class="card-img-top" alt="...">
                    <div class="card-body">
                      <h5 class="card-title">Air interdiction</h5>
                      <p class="card-text">In this role the Eurofighter Typhoon is configured for ground attacks and even though it is equipped with a targeting pod and up to 7 ground attack weapons, it carries still 3 BVR and 2 SR missiles.</p>
                      
                    </div>
                </div>
            </div>
            <div class="col-12 col-md-6 col-lg-4 mb-4">
                <div class="card" style="width: 18rem;">
                    <img src="./assets/img/mig3.jpg" class="card-img-top" alt="...">
                    <div class="card-body">
                      <h5 class="card-title">Close air support</h5>
                      <p class="card-text">The recent integration contract for the Brimstone has strengthened the CAS capabilities of the Eurofighter Typhoon since it can now engage in combat with a reduced risk of collateral damages of non-combatant or friendly forces.</p>
                      
                    </div>
                </div>
            </div>
            
        </div>
    </section>
	
CSS

    /* cards */
    
    #speakers img {
        height: 348px;
        object-fit: cover;
    } 
    

------------

### PASTILLAS DE TEXTO

[Badges](https://getbootstrap.com/docs/5.0/components/badge/ "Badges")

HTML

    <div class="badges">
        <span class="badge bg-warning">Combat</span>
        <span class="badge bg-info">Aircraft</span>
    </div>
CSS

    .badges{
        text-align: right;
    }


<img src="https://static.platzi.com/media/user_upload/badges-80335d48-d52b-4386-9eb3-ecdf7de49bf9.jpg" alt="badges">
------------


### AGREGANDO UN CONTENEDOR DE ANCHO COMPLETO

[Contenedor fluido](https://getbootstrap.com/docs/5.0/layout/containers/ "Contenedor fluido")

HTML



```
   <!-- PLACE AND DATE -->

    <section id="place-time">
      <div class="container-fluid">
        <div class="row">
          <div class="col-12 col-lg-6 pt-3 pl-0 pr-0"> <!-- padding left padding right -->
            <img src="assets/img/honolulu.jpg" alt="City"></div>
          
          <div class="col-12 col-lg-6 pt-4 pb-4 align-self-center">
            <h2 >
              HONOLULU OCTUBRE 3021
            </h2>
            <p>
              The Eurofighter Typhoon is the world's most modern swing-role fighter.
            </p>
            <a href="#" class="btn btn-outline-light" target="_blank">Conoce más</a>
          </div>
        </div>
      </div>
    </section>

    <!-- PLACE AND DATE --> 
```


CSS



```
/* place and date */

#place-time {
    background-color: var(--secondary-color);
    color: var(--just-white);
}


#place-time img{
    max-width: 100%;
}

/* place and date */
```


------------

### AGREGANDO UN TOOLTIP

[Tooltip](https://getbootstrap.com/docs/5.0/components/tooltips/ "Tooltip")

Un tooltip (también llamada descripción emergente) es una herramienta de ayuda visual, que funciona al situar el cursor sobre algún elemento gráfico, mostrando una ayuda adicional para informar al usuario de la finalidad del elemento sobre el que se encuentra.

Los tooltip son una variación de los globos de ayuda y es un complemento muy usado en programación y diseño, dado que proporcionan información adicional sin necesidad de que el usuario la solicite de forma activa.

**HTML**

	<div class="col text-center">
	Llena el formulario y participa.
	Quizá hoy seas tu la nueva estrella de la <abbr data-bs-toggle="tooltip" data-bs-placement="top" title="El arte de crear y organizar sonidos y silencios">música!</abbr>
	</div>

**En javascript**

	var tooltipTriggerList = [].slice.call(document.querySelectorAll('[data-bs-toggle="tooltip"]'))
	var tooltipList = tooltipTriggerList.map(function (tooltipTriggerEl) {
	  return new bootstrap.Tooltip(tooltipTriggerEl)
	})

------------



------------



[========]