<template>
  <div class="col-4">
    <div class="card">
      <img :src="juego.background_image" class="card-img-top" alt="..." />
      <div class="card-body">
        <h5 class="card-title font-weight-bold text-danger">{{ juego.name }}</h5>
      </div>
      <ul class="list-group list-group-flush">
        <li class="list-group-item">{{ juego.rating }}</li>
        <li class="list-group-item">{{ juego.released }}</li>
        <li class="list-group-item">{{ juego.updated }}</li>
      </ul>
      <div class="card-body">
        <button class="btn btn-info" @click="setOpenModalOpinion(index)">
          Dejanos tu opinión
        </button>
      </div>
    </div>
  </div>
</template>

<script>
import { mapActions } from "vuex";
export default {
  name: "GamesCard",
  props: {
    juego: {
      type: Object,
      default() {
        return {};
      },
    },
    index: {
      type: Number,
      default() {
        return 0;
      },
    },
  },
  methods: {
    ...mapActions(["setOpenModalOpinion"]),
  },
};
</script>

