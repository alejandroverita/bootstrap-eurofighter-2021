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



[========]