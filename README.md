<!DOCTYPE html>
<html>
    <head>
        <title>PET ACCESORIES</title>
        <meta name="viewport" content="width=device-width, initial-scale=1">
        <style>
            * {box-sizing: border-box;}
            body  { font-family: verdana, sans-serif;}
            .mySlides {display: none;}
            img {vertical-align: middle;}
            /* Contenedor del Carrucel */
            .contenedor-slideshow {
                max-width: 500px;
                position: relative;
                margin: auto;
            }
            /* Textos Slides */
            .texto {
                color: #f2f2f2;
                font-size: 15px;
                padding: 8px 12px;
                position: absolute;
                bottom: 8px;
                width: 100%;
                text-align: center;
            }
            /* Numero Texto (1/3 etc...) */
            .numerotexto {
                color: #f2f2f2;
                font-size: 12px;
                padding: 8px 12px;
                position: absolute;
                top: 0;
            }
            /* Los puntos/bullets/indicadores */
            .punto {
                height: 10px;
                width: 10px;
                margin: 0 2px;
                background-color: #bbb;
                border-radius: 25%;
                display: inline-block;
                transition: background-color 0.6s ease;
            }
            .activo {
                background-color: #717171;
            }
            /*Animacion desvanecer */
            .desvanecer {
                -webkit-animation-name: fade;
                -webkit-animation-duration: 1.5s;
                animation-name: fade;
                animation-duration: 1.5s;
            }
            @-webkit-keyframes fade {
                from {opacity: .4}
                to {opacity: 1}
            }
            @keyframes fade {
                from {opacity: .4}
                to {opacity: 1}
            }
            /* en pantallas pequeñas se reduce el tamaño del texto */
            @media only screen and (max-width: 300px) {
                .texto {font-size: 11px}
            }
            .logotipo {
            position:absolute;
            width: 145px;
            height: 136px;
            left: 0px;
            top: -3px;
            }
            h1 {
                text-align: center; font-family: Belgrano;}
            p {text-align: center;font-family: Righteous;}

            .boton {
            background-color: rgba(62, 73, 72, 0.5);
            border:none;
            color:white;
            padding:  15px 32px;
            text-align: center;
            text-decoration: none;
            display:inline-block;
            font-size: 16px;
            margin: 4px  2px;
            cursor: pointer;
            -webkit-transition-duration: 8.4s;
            transition-duration: 0.4s;
            }

        .boton1:hover {border-radius: 12px; 
            box-shadow: 0 12px 16px 0 rgba(0,0,0,0.24),0 17px 50px 0 rgba(0,0,0,0.19) ;}
        .boton2:hover {border-radius: 12px;
            box-shadow: 0 12px 16px 0 rgba(0,0,0,0.24),0 17px 50px 0 rgba(0,0,0,0.19) ;}
        .boton3:hover {border-radius: 12px;
            box-shadow: 0 12px 16px 0 rgba(0,0,0,0.24),0 17px 50px 0 rgba(0,0,0,0.19) ;}
        .boton4:hover {border-radius: 12px;
            box-shadow: 0 12px 16px 0 rgba(0,0,0,0.24),0 17px 50px 0 rgba(0,0,0,0.19) ;}
        .boton5:hover {border-radius: 12px;
            box-shadow: 0 12px 16px 0 rgba(0,0,0,0.24),0 17px 50px 0 rgba(0,0,0,0.19) ;}
        .boton6:hover {border-radius: 12px;
            box-shadow: 0 12px 16px 0 rgba(0,0,0,0.24),0 17px 50px 0 rgba(0,0,0,0.19) ;}
        .table {position: absolute; width: 150px; height: 213px; left: 50px; top: 207px;}
        </style>
    </head>
<body background="FONDO4.jpg" bgcolor="FFCECB">
<table width="550" bgcolor=transparent align=center>
<tr>
<td>
<h1 style="color:000000"> BIENVENIDOS </h1>
<br> LOS MEJORES ACCESORIOS PARA TU MASCOTA DE LA MEJOR CALIDAD <br>
</td>
</tr>
</table>
<form class="table">
 <table width="150" bgcolor=transparent align=absolute>
 <tr>
 <td>
 <a href="PERROS.HTML"><boton class="boton boton1">PERROS</boton></a>
 <a href="GATOS.HTML"><boton class="boton boton2">GATOS</boton></a>
 <a href="PECES.HTML"><boton class="boton boton3">PECES</boton></a>
 <a href="TORTUGAS.HTML"><boton class="boton boton4">TORTUGA</boton></a>
 <a href="AVES.HTML"><boton class="boton boton5">AVES</boton></a>
 <a href="ROEDORES.HTML"><boton class="boton boton6">ROEDORES</boton></a>
</td>
</tr>
</table>
</form>
 
<div class="logotipo">
 <img src="logotipo.jpg" style="width:100%">
</div>

<div class="contenedor-slideshow">
 <div class="Carrusel fade">
 <div class="numerotexto">1</div>
 <img src="perrito_acostado.jpg" style="width:100%">
</div>

<div class="Carrusel fade">
 <div class="numerotexto">2</div>
 <img src="perro_dover.jpg" style="width:100%">
</div>

<div class="Carrusel fade">
 <div class="numerotexto">3</div>
 <img src="perro_arbol.jpg" style="width:100%">
</div>

<div class="Carrusel fade">
 <div class="numerotexto">4</div>
 <img src="perro_boxer.jpg" style="width:100%">
</div>
</div>

<br>
 <div style="text-align:center">
 <span class="punto"></span>
 <span class="punto"></span>
 <span class="punto"></span>
  <span class="punto"></span>
</div>
     <script>
        var slideIndex = 0;
            showSlides();
            function showSlides() {
                var i;
                var slides = document.getElementsByClassName("Carrusel");
                var puntos = document.getElementsByClassName("punto");
                for (i = 0; i < slides.length; i++) {
                    slides[i].style.display = "none";
                }
                slideIndex++;
                if (slideIndex > slides.length) {slideIndex = 1}
                for (i = 0; i < puntos.length; i++) {
                    puntos[i].className = puntos[i].className.replace(" activo "," ");
                }
                slides[slideIndex-1].style.display = "block";
                puntos[slideIndex-1].className += " activo ";
                setTimeout(showSlides, 2000); //cambia la imagen cada dos segundos
            }
        </script>
</body>
</html>
