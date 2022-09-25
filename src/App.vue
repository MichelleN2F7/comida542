<template>
  <div>
    <header>
      <nav>
          <ul>
            <li><a href=""> </a></li>
            <li><a href=""> </a></li>
            <li><a href=""> </a></li>
            <li><a href=""> </a></li>
            <li><a href=""> </a></li>
            <li><a href=""> </a></li>
            <li><a href="">Bebidas</a></li>
            <li><a href="">Hamburguesas</a></li>
            <li><a href="">Burritos</a></li>
            <li><a href="">Papas</a></li>
            <li><a href="#">Michelle Negrellos Fong</a></li>
            <li><a href="">4 "B"</a></li>
          </ul>
        </nav>
    </header>
  </div>

  <div>
    <h1>Fonk's Fast Food </h1>
    <hr>
  </div>
  <div class="container">
    
    <slot />
    <card url="https://www.saborusa.com/wp-content/uploads/2019/12/origen-de-la-pizza-1.jpg" nombre="Pizza" descripcion="Rica pizza tamaño grande de peperoni con motzarela." precio="122.00" />

    <card url="https://images.hola.com/imagenes/cocina/noticiaslibros/20210528190401/dia-internacional-hamburguesa-recetas-2021/0-957-454/dia-hamburguesa-m.jpg" nombre="Hamburguesa" descripcion="Hamburguesa tradicional, con carne de res y queso" precio="62.00" />

    <card url="https://th.bing.com/th/id/R.ef56ce7eb66714ca35d611282992472c?rik=v7cPpyNKrjeP%2bw&pid=ImgRaw&r=0" nombre="Burrito" descripcion="Burritos de fajitas de pollo con rajas y elote" precio="78.00" />

    <card url="https://cdn2.cocinadelirante.com/sites/default/files/images/2021/09/porque-comer-un-hot-dog-reduce-la-vida.jpg" nombre="Hot dog" descripcion="Hot dog tradicional con pan integral" precio="15.00" />

    <card url="https://th.bing.com/th/id/OIP.YVHdS9V7FGaqYXeqxoMF_wHaIe?pid=ImgDet&rs=1" nombre="Alitas" descripcion="Ricas docena de alitas en salsa BBQ" precio="82.00" />

    <card url="https://cdn2.cocinadelirante.com/sites/default/files/styles/gallerie/public/images/2020/06/papas-fritas-con-maicena-facil.jpg" nombre="Papas fritas" descripcion="Papas naturales estilo francesa con paprika" precio="25.00" /> 
    
  </div>

  <div>
    <!-- Site footer -->
    <footer class="site-footer" style="background-color: #9d6058">
              <!-- Section: Links -->
          <section class="mt-5">
                <!-- Grid row-->
              <div class="row t-c d-flex pt-5">
                  <div class="col-md-2">
                      <h5>About us</h5>
                  </div>

                  <div class="col-md-2">
                      <h5>Contact us</h5>
                  </div><!--cold-md-2 Aw-->
                  
                  <div class="col-md-2">
                      <h5>Products</h5>
                  </div><!--cold-md-2 Pr-->
                  
                  <div class="col-md-2">
                      <h5>Services</h5>
                  </div><!--cold-md-2 H-->
                  
                  <div class="col-md-2">
                      <h5>History</h5>
                  </div>
              </div>
          </section>
          <hr class="my-5" />
  
          <section class="mb-5"> <!-- Section: Text -->
            <div class="row d-flex justify-content-center">
              <div class="col-lg-8">
                <p>
                  Lorem ipsum dolor sit amet consectetur adipisicing elit. Sunt
                  distinctio earum repellat quaerat voluptatibus placeat nam,
                  commodi optio pariatur est quia magnam eum harum corrupti
                  dicta, aliquam sequi voluptate quas.
                </p>
              </div>
            </div>
          </section><!-- Section: Text -->
          
          <div class="text-center p-3" style="background-color: rgba(0, 0, 0, 0.2)">
              © 2020 Copyright:
              <a class="text-white" href="">
                  FonkFastFood.com
              </a>
              <a href="" target="_blank">Michelle Negrellos Fong 4B</a>.
          </div> 
      </footer>
  </div>
</template>

<style>
  nav{
    float: center;
    background-color: #6e3415;
  }

  nav ul {
    list-style: none;
    overflow: hidden; 
  }

  nav ul li {
    float: left;
    font-family: Arial, sans-serif;
    font-size: 16px;
  }

  nav ul li a {
    display: block; /* Convertimos los elementos a en elementos bloque para manipular el padding */
    padding: 20px;
    color: rgb(255, 255, 255);
    text-decoration: none;
  }

  nav ul li:hover {
    background: #FFAC41;
  }

  h1{
    text-align: center;
  }
  
 /*------Footer ------------*/
 @import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');

  .site-footer
  {
    background-color:#000000;
    padding:0.5px 0 1px;
    font-family: 'Roboto', sans-serif;
    font-size: 18px;
    line-height:24px;
    margin-top: 1rem;
    color:#ffffff;
  }
  .site-footer hr
  {
    border-top-color:#e8cea0;
    opacity:0.5
  }
  .site-footer hr.small
  {
    margin:20px 0
  }  
  .site-footer h6
  {
    color:#fff;
    font-size:18px;
    text-transform:uppercase;
    margin-top:5px;
    letter-spacing:2px;
    margin-left: 3px;
  }
  .site-footer a
  {
    color:#ffffff;
    text-align: center;
  }
  .site-footer a:hover
  {
    color:#fff200;
    text-decoration:none;
  }
  .footer-links
  {
    padding-left:0;
    list-style:none;
    text-align: center;
  }
  .footer-links li
  {
    display:block;
    text-align: center;
  }
  .footer-links a
  {
    color:#737373
  }
  .footer-links a:active,.footer-links a:focus,.footer-links a:hover
  {
    color:#fff700;
    text-decoration:none;
  }
  .footer-links.inline li
  {
    display:inline-block
  }
  
  .copyright-text
  {
    margin:1px;
  }
</style>
  
<script>
  import Card from "./components/Card.vue"
  
  export default {
    components:{
      Card,
    },
  };
</script>