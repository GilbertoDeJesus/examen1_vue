<script setup>
import Header_nav from './components/Header_nav.vue';
import Products from './components/Products.vue';
import Footer from './components/Footer.vue';
</script>

<template>

  <Header_nav url="https://cdn.pixabay.com/photo/2017/06/13/22/31/logo-2400338_960_720.png"
    nombreEmpresa="La cocina de Elisa" nombreAlumno="Gilberto Angel de Jesus Suarez" grupo="10 A" />

  <main>
    <div class="jumbotron">
      <div class="container">
        <h1 class="display-4">Nuestros platos</h1>
        <p class="lead">Inicio / Nuestros platos</p>
      </div>
    </div>
    <div class="container text-center">
      <div class="alert alert-primary w-100" role="alert">
        Telefono para pedidos: 952 03 99 50
      </div>
      <h2 class="pt-2 pb-2">Ensaladas y entrantes</h2>
      <div class="row">
        <Products url="https://upload.wikimedia.org/wikipedia/commons/4/4b/Comida_en_la_Feria_del_Mole_2014_10.JPG" nombre="Mole" precio="$10.00" descripcion="Comida" />
        <Products url="https://assets.tmecosys.com/image/upload/t_web767x639/img/recipe/ras/Assets/BE035512-0E75-41ED-B1C2-EA9A8C6062E8/Derivates/FBEEFA5F-A1B5-47B2-B632-BFD0506D00AA.jpg" nombre="Pozole" precio="$60.00" descripcion="Comida" />
        <Products url="https://www.cardamomo.news/__export/1645307144067/sites/debate/img/2022/02/19/barbacoa_estilo_hidalgo.png_423682103.png" nombre="Barbacoa" precio="$40.00" descripcion="Comida" />
        <Products url="https://cdn2.cocinadelirante.com/sites/default/files/styles/gallerie/public/images/2020/09/como-se-hacen-las-carnitas-facil.jpg" nombre="Carnitas" precio="$50.00" descripcion="Comida" />
        <Products url="https://laroussecocina.mx/wp-content/uploads/2022/05/Tlayuda-Marcos-Castillo-e1652445509465.png" nombre="Tlayudas" precio="$30.00" descripcion="Comida" />
        <Products url="https://bakeitwithlove.com/wp-content/uploads/2022/04/shredded-chicken-tacos-sq.jpg" nombre="Tacos" precio="$20.00" descripcion="Comida" />
      </div>
    </div>
  </main>

  <Footer />
</template>

<style scoped>
header {
  line-height: 1.5;
}

.jumbotron {
  width: 100vw;
}

main {
  width: 100vw;
}
</style>
