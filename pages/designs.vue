<template>
  <div id="designs">
    <Header></Header>

    <section class="more-designs__container">
      <p class="more-designs__header">More Designs</p>
      <p class="more-designs__text">
        These are some of my other commissioned design works, consisting of
        mobile and web designs.
      </p>

      <section class="design__images">
        <div class="design__container">
          <img src="../assets/images/design-1.png" alt="" />
          <p class="design__caption">MAX Delivery Admin Dashboard</p>
        </div>
        <div class="design__container">
          <img src="../assets/images/design-2.png" alt="" />
          <p class="design__caption">Megalectrics Radio App</p>
        </div>
        <div class="design__container">
          <img src="../assets/images/design-3.png" alt="" />
          <p class="design__caption">MAX Delivery Driver Web App</p>
        </div>
        <div class="design__container">
          <img src="../assets/images/design-4.png" alt="" />
          <p class="design__caption">Fieldinsight website</p>
        </div>
      </section>
    </section>
    <SubFooter></SubFooter>
  </div>
</template>

<script>
import Header from "../components/Header.vue";
import SubFooter from "../components/SubFooter.vue";
export default {
  components: {
    Header,
    SubFooter,
  },
};
</script>

<style scoped>
#designs {
  background-image: url("../assets/images/lines-for-web.svg");
  background-repeat: no-repeat;
  background-position: top center;
}

.more-designs__container {
  max-width: 109.2rem;
  margin: 0 auto;
  padding-top: 7rem;
  padding-bottom: 5rem;
  padding-left: 121px;
  padding-right: 121px;
}

.more-designs__header {
  font-family: "Graphik-SemiBold";
  font-size: 2rem;
  font-weight: 600;
  line-height: 4.5rem;
  margin-bottom: 1.5rem;
}

.more-designs__text {
  font-family: "Graphik-Regular";
  font-size: 1.3rem;
  font-weight: 300;
  line-height: 3rem;
  margin-bottom: 3rem;
}

.design__images {
  gap: 68px;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(500px, 1fr));
}

.design__images img {
  max-width: 100%;
}

.design__caption {
  font-family: "Graphik-Regular";
  margin-top: 1rem;
  font-size: 18px;
  font-weight: 900;
}

@media screen and (min-width: 1024px) {
  .design__images {
    gap: 20px;
    grid-template-columns: repeat(auto-fit, minmax(380px, 1fr));
  }
}

@media screen and (min-width: 1440px) {
  .design__images {
    gap: 76px;
    grid-template-columns: repeat(auto-fit, minmax(550px, 1fr));
  }

  .design__images img {
    max-width: 100%;
  }
}

@media screen and (max-width: 980px) {
  .more-designs__container {
    padding-left: 64px;
    padding-right: 64px;
  }

  .design__images {
    grid-template-columns: 1fr;
  }

  .design__images img {
    max-width: 100%;
  }
}

@media screen and (max-width: 768px) {
  .more-designs__container {
    padding-left: 32px;
    padding-right: 32px;
  }
}

@media screen and (max-width: 540px) {
  #designs {
    background-image: url("../assets/images/lines-for-mobile.svg");
    background-repeat: no-repeat;
    background-position: top center;
    /* height: 100%; */
  }

  .more-designs__header {
    font-size: 26px;
    font-weight: 300;
    line-height: 50px;
  }

  .more-designs__text {
    font-size: 18px;
    font-weight: 300;
    line-height: 48px;
  }

  .design__caption {
    font-size: 18px;
    font-weight: 300;
    line-height: 48px;
  }
}

@media screen and (max-width: 320px) {
  .more-designs__header {
    font-size: 20px;
    font-weight: 300;
    line-height: 40px;
  }

  .more-designs__text {
    font-size: 15px;
    font-weight: 300;
    line-height: 40px;
  }

  .design__caption {
    font-size: 15px;
    font-weight: 300;
    line-height: 40px;
  }
}

@media screen and (max-width: 280px) {
  .more-designs__container {
    padding-left: 16px;
    padding-right: 16px;
  }
}
</style>
