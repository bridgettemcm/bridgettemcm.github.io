# 3D-Cube-Animation-with-Image
body{
  background: #303030;
}
.contenedor {
  -webkit-perspective: 500px;
  perspective: 500px;
  perspective-origin: 50% 50%;
}

.cube, .cube .card{
  height: 290px;
  width: 290px;
}

.cube {
  -webkit-transform-style: preserve-3d;
  transform-style: preserve-3d;

  -webkit-transform: rotateX(-30deg) rotateY(30deg);
  transform: rotateX(-30deg) rotateY(-30deg);

  margin: 150px auto;

  -webkit-animation: giro 20s infinite linear;
  animation: giro 20s infinite linear;
}

.cube .card {
  position: absolute;
  border: 5px solid #ccc;
  opacity: 0.85;
  transition: 0.2s;
}
/* Pause animation on hover */
.cube:hover{
    animation-play-state: paused;
}
.cube:hover .card{
   opacity: 1;
   transition: 0.2s;
}

/*card frontal*/
.cube .card:nth-child(1) {
  -webkit-transform: translateZ(150px);
  transform: translateZ(150px);
}
/*card posterior*/
.cube .card:nth-child(2) {
  -webkit-transform: rotateY(180deg) translateZ(150px);
  transform: rotateY(180deg) translateZ(150px);
}
/*card izquierda*/
.cube .card:nth-child(3) {
  -webkit-transform: rotateY(-90deg) translateZ(150px);
  transform: rotateY(-90deg) translateZ(150px);
}
/*card derecha*/
.cube .card:nth-child(4) {
  -webkit-transform: rotateY(90deg) translateZ(150px);
  transform: rotateY(90deg) translateZ(150px);
}
/*card superior*/
.cube .card:nth-child(5) {
  -webkit-transform: rotateX(90deg) translateZ(150px);
  transform: rotateX(90deg) translateZ(150px);
}
/*card inferior*/
.cube .card:nth-child(6) {
  -webkit-transform: rotateX(-90deg) translateZ(150px);
  transform: rotateX(-90deg) translateZ(150px);
}

@-webkit-keyframes giro {
    0% { -webkit-transform: rotateX(-45deg) rotateY(0deg); }
    50% { -webkit-transform: rotateX(45deg) rotateY(360deg); }
    100% { -webkit-transform: rotateX(-45deg) rotateY(720deg); }
}

@keyframes giro {
    0% { transform: rotateX(-45deg) rotateY(0deg); }
    50% { transform: rotateX(45deg) rotateY(360deg); }
    100% { transform: rotateX(-45deg) rotateY(720deg); }
}

@-webkit-keyframes giro360 {
    0% { -webkit-transform: rotateX(  0deg) rotateY(  0deg); }
  100% { -webkit-transform: rotateX(360deg) rotateY(360deg); }
}

@keyframes giro360 {
    0% { transform: rotateX(  0deg) rotateY(  0deg); }
  100% { transform: rotateX(360deg) rotateY(360deg); }
}
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1"> 
    <meta name="viewport" content="width=device-width, initial-scale=1.0"> 
    <title>CSS3 3D Cube Animation with Image Example</title>
    <meta name="author" content="Codeconvey" />
    
    <!-- Style CSS -->
    <link rel="stylesheet" href="css/style.css">
    
    <!--Only for demo purpose - no need to add.-->
    <link rel="stylesheet" type="text/css" href="css/demo.css" />
	
</head>
<body>
		
<div class="ScriptTop">
    <div class="rt-container">
        <div class="col-rt-4" id="float-right">

            <!-- AD HERE -->
            
        </div>
        <div class="col-rt-2">
            <ul>
                <li><a href="https://codeconvey.com/css3-3d-cube-animation-with-image">Back to Tutorial</a></li>
            </ul>
        </div>
    </div>
</div>

<header class="ScriptHeader">
    <div class="rt-container">
    	<div class="col-rt-12">
        	<div class="rt-heading">
            	<h1>CSS3 3D Cube Animation with Image Example</h1>
                <p>Cube animated clickable images with CSS3.</p>
            </div>
        </div>
    </div>
</header>

<section>
    <div class="rt-container">
          <div class="col-rt-12">
              <div class="Scriptcontent">
              
<!-- partial:index.partial.html -->
<div class="contenedor"> 
			<div class="cube">
				<div class="card">
                    <a href="#">
					<img src="img/image-1.jpg" title="Soto y Caldevilla de Valdeón" alt="Soto y Caldevilla de Valdeón" height="290px" width="290px" >
				  </a>
                        </div>
				<div class="card">
                    <a href="#">
					<img src="img/image-2.jpg" title="Un poco de nieve en agosto" alt="Un poco de nieve en agosto" width="290px" height="290px">
				  </a>
                        </div>
				<div class="card">
                    <a href="#">
					<img src="img/image-3.jpg" title="Un rebeco" alt="Un rebeco" width="290px" height="290px">
				  </a>
                        </div>
				<div class="card">
                    <a href="#">
					<img src="img/image-4.webp" title="Posada de Valdeón" alt="Posada de Valdeón" width="290px" height="290px">
				  </a>
                        </div>
				<div class="card">
                    <a href="#">
					<img src="img/image-5.jpg" title="Refugio de Pantivalles" alt="Refugio de Pantivalles" width="290px" height="290px">
				  </a>
                        </div>
				<div class="card">
                    <a href="#">
					<img src="img/image-6.jpg" title="Unas montañas" alt="Unas montañas" width="290px" height="290px">
                    </a>
				</div>
                    
			</div>
		</div>
<!-- partial -->
    		
           
    		</div>
		</div>
    </div>
</section>
     

   <!-- ANALYTICS -->

	</body>
</html>
