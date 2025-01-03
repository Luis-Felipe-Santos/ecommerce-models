<template>
  <section class="banner-pitchbar">
    <div class="banner">
      <vueper-slides class="slide" fade :touchable="false" :fixed-height="350">
        <vueper-slide
          v-for="(slide, i) in slides"
          :key="i"
          :image="slide.image"
        />
      </vueper-slides>
    </div>
    <div class="pitchbar">
      <div class="pitchbar-items">
        <img src="../assets/Ícone-frete.svg" alt="" />
        <div class="txt-span">
          <span>Frete Grátis</span>
          <p>Frete grátis em todos os pedidos</p>
        </div>
      </div>
      <div class="pitchbar-items">
        <img src="../assets/icone-cartao.svg" alt="" />
        <div class="txt-span">
          <span>Parcele em até 10x</span>
          <p>Sem juros no cartão de crédito</p>
        </div>
      </div>
      <div class="pitchbar-items">
        <img src="../assets/icone-dinheiro.svg" alt="" />
        <div class="txt-span">
          <span>Devolução de Dinheiro</span>
          <p>Garantia de devolução de 7 dias</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import { VueperSlides, VueperSlide } from "vueperslides";
import "vueperslides/dist/vueperslides.css";

export default {
  name: "HomePage",
  components: { VueperSlides, VueperSlide },

  data: () => ({
    slides: [
      {
        image: require("@/assets/Banner.svg"),
      },
      {
        image: require("@/assets/Banner2.svg"),
      },
      {
        image: require("@/assets/Banner3.svg"),
      },
    ],
  }),
};
</script>

<style scoped>
.banner-pitchbar {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  gap: 12px;
}
.banner {
  width: 100%;
  height: 350px;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 24px;
}
.slide {
  width: 100%;
  max-width: 1216px;
  height: 350px;
  overflow: hidden;
  border-radius: 32px;
}
.pitchbar {
  display: flex;
  gap: 8px;
  width: 100%;
  max-width: 1216px;
  height: 56px;
  padding: 8px 16px 8px 16px;
}
.pitchbar-items {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 397.33px;
  height: 56px;
  background-color: #eff8ff;
  border-radius: 14px;
  gap: 8px;
}
.pitchbar-items span {
  color: #1570ef;
  font-size: 14px;
  line-height: 20px;
  font-weight: 600;
}
.pitchbar-items p {
  color: #b3b9c6;
  font-size: 12px;
  line-height: 14.52px;
  font-weight: 400;
}
</style>
