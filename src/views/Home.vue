
<template>
  <div>
    <header class="container text-center py-5">
      <h1>Encuentra aquí los Juegos Disponibles</h1>
    </header>
    <section class="container">
      <GamesCardList />
    </section>
  </div>
</template>

<script>
import GamesCardList from "@/components/GamesCardList";

export default{
    name: "Home",
    components:{
        GamesCardList,
    }
};

</script>