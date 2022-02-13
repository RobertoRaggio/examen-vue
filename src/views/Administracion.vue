<template>
  <div>
    <header class="container text-center py-5">
      <h1>Administrador de los comentarios</h1>
    </header>
    <section class="container">
      <AdminOpinion />
    </section>
  </div>
</template>

<script>
import AdminOpinion from "@/components/AdminOpinion";
export default {
  name: "Administracion",
  components: {
    AdminOpinion,
  },
};
</script>
