<template>
  <div class="card col-lg-6">
    <span class="icon" v-html="card.img"></span>
    <span class="title">{{ card.title }}</span>
    <span class="desc">{{ card.desc }}</span>
  </div>
</template>

<script>
export default {
  name: "CardServices",
  props: ["card"],
};
</script>

<style lang="scss" scoped>
.card {
  display: flex;
  flex-direction: column;
  justify-content: start;
  align-items: center;
  max-width: 277px;
  padding: 30px;
  border-radius: 30px;
  background-color: #fff;
  box-shadow: 7px 12px 43px 0px rgba(0, 0, 0, 0.14);

  .title {
    color: #5fe26c;
    text-align: center;
    font-family: Inter;
    font-size: 24px;
    font-style: normal;
    font-weight: 700;
    line-height: normal;
    text-transform: uppercase;
    margin: 30px 0 25px 0;
    width: 120%;
  }

  .desc {
    color: #90bd95;
    text-align: center;
    font-family: Inter;
    font-size: 20px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
  }
}
</style>
