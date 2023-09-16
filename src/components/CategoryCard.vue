<script>
export default {
  name: "CategoryCard",
  props: ["category"],
};
</script>

<template>
  <div class="card col-xl-3 col-lg-4 col-md-6 col-sm-12 col-xs-12">
    <div class="card-header">
      <img :src="category.img" alt="" />
    </div>
    <div class="card-body">
      <p>{{ category.title }}</p>
      <span>({{ category.items }})</span>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.card {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 10px;
  max-width: 325px;
  max-height: 320px;
  background-color: #fff;
  border-radius: 40px;
  box-shadow: 2px 10px 30px 0px rgba(0, 0, 0, 0.1);
  padding: 25px 0;

  .card-header {
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #c1f1c6;
    border-radius: 50%;
    width: 153px;
    height: 153px;
    margin-top: 20px;
    overflow: hidden;

    img {
      width: 139px;
      height: 102px;
      border-radius: 50%;
      object-fit: contain;
    }
  }

  .card-body {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 15px;

    p {
      margin: 0;
      padding: 0;
      color: #1e1e1e;
      text-align: center;
      font-family: Inter;
      font-size: 30px;
      font-style: normal;
      font-weight: 600;
      line-height: normal;
    }

    span {
      margin: 0;
      padding: 0;
      color: #555;
      text-align: center;
      font-family: Inter;
      font-size: 22px;
      font-style: normal;
      font-weight: 500;
      line-height: normal;
      margin-bottom: 20px;
    }
  }
}
</style>
