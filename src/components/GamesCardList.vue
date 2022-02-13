<template>
  <div class="row">
    <GamesCard
      v-for="(juego, index) in juegos"
      :key="index"
      :juego="juego"
      :index="index"
    />
    <ModalComments />
  </div>
</template>

<script>
import { mapState } from "vuex";
import GamesCard from "@/components/GamesCard";
import ModalComments from "@/components/ModalOpinion";
export default {
  name: "GamesCardList",
  components: {
    GamesCard,
    ModalComments,
  },
  computed: {
    ...mapState(["juegos"]),
  },
};
</script>