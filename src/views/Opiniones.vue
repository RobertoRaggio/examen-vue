<template>
  <div>
    <header class="container text-center py-5">
      <h1>Opiniones</h1>
    </header>
    <section class="container">
      <PeopleOpinion />
    </section>
  </div>
</template>

<script>
import PeopleOpinion from "@/components/PeopleOpinion";
export default {
  name: "Opiniones",
  components: {
    PeopleOpinion,
  },
};
</script>