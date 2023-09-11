<script>
import CategoryCard from "./CategoryCard.vue";
export default {
  name: "CategoriesVue",
  components: { CategoryCard },
  data: () => {
    return {
      categories: [
        {
          id: 1,
          title: "Main Dish",
          items: "86 dishes",
          img: "https://s3-alpha-sig.figma.com/img/e86f/35a4/f2648ec1cc19cd09ba4a72b5f4a76a2f?Expires=1694390400&Signature=P6dFCZUw-Ae5fS94vbKMJF6M~1kYwNWGriCEU4gFsvudsp9irpuTLkp0oQsksYs0TX9n37R8T9Ebu8GvO-fPYp1AVta1WXA2vmEC~zJ1fauycdqhHmekGRBYhynd3RBUaHgFXuq4lxuaP9GfRztuXDkTEi6h1OaCiLtbngsCsRo0nskpjIMMv787m8w4TeZpNuwfw-PpOYLixy~izG3tIqF1h2VGSRRJWA~2R0IJFOH-Nk~7Uq1G0tPOpIoZtmkV8rylqsR8FN6dUzpEXAtYYoyQxa2PC-CvrREmVELEbXSXyW0D7qwFpuWirJNLP7lS-BYuG555iypQRIYitew8Vw__&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4",
        },
        {
          id: 2,
          title: "Break Fast",
          items: "12 break fast",
          img: "https://s3-alpha-sig.figma.com/img/9ac5/7848/92cebe7826b91979d7ec7154dc714870?Expires=1694390400&Signature=C7fTQF82ufOzDZDkoGSb1hMnwHuqpnoJNoBnMHsl2lkgK4pNDmUh73dqTqScYssPEdoVnYUydrbGutrzYpup9PO2axllqAQGo4N9TxTvmsIwXTG2g95b7bBSO0QrgKmc8E2aHutJSDk2NA3-ayvSW6N7oI2jxFx1tIvjTP9KaIZYJKVnJYpEmYLxDKJ~Dw0RjXx4el97pyNS~5~JCafbTPe0ZeMPuXraTEUkNAbP4yEbAorZAm6MWDJxqyA53YLBSABRbkIy1EUUaHrJmN5NGBPUSgaUa4E7Lg4bc57MqfklQj8pgvR0W9Xz556S49FIGaLJXNNqMGMFdsxo8nYOsw__&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4",
        },
        {
          id: 3,
          title: "Dessert",
          items: "48 dessert",
          img: "https://s3-alpha-sig.figma.com/img/cd96/980b/00a7e066cf0ba10fb8fcd8d7604eb761?Expires=1694390400&Signature=LK2DWHF4Z1GpvDWhVNGjVM74RRihGZeN-K9X6sOwHa0~-I5yBnfG1XYidFi~ygsn-izV10Tye5eU--uCKyNE5swu6BApUfak4x-Jytuf~JzpSX-tm2apk3K0u2Dmmy1RwmX2AMiaeyukTab2A2hlVacSUL4CUR3NjfjjyJ41HQ-5UI8HotIs6IsUepn-DYMXnqnkT9D4LpP2uvvOYcRlZqxwqA6BpHkppM0vT17pKh~zjlCiNjnZq5vb4Whz7Kq2CPv1YoaQqsdmHvpvms2uZg-j9ZT574ZTEq0Jqux5LEpGDa9lmU1WePADFKeFK6ywagLzYnNPE9icXJ3v1LnF2Q__&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4",
        },
        {
          id: 4,
          title: "Browse All",
          items: "255 Items",
          img: "https://s3-alpha-sig.figma.com/img/6b05/0fed/66e0e5da0f9f7eab54d2ff4a36225a83?Expires=1694390400&Signature=ElHRcD5z2dop6tNls8b7hdnJLFlsJwdeCFi3ToY2gO94TeopG4xlU43eReofNARqaIw5ogvfbd5U3K-0pRQE1s3Jl-yjSd2F3I6KyQKeGQR8mVvl2Tqm5mCbSGFnhn8U3kJanBois23VC10c9HKDYYA3vUOL5onMXWrNiu2FdVrgZBbXa-sKLkMXQgsIrmbkYFOZRlknIhQMztotYDjEhtVfNQFYnpInrtiUjEFaMrJppFfsRlvd4RdIZwNdrQQqGClGULzb4i5s28QCvacs0eZLDz39Ek1VNEWNqR9pStcq9A7Qw6Sz1a9TJgkrrkaIQyQfiMl8YwesWIQPTh1vkg__&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4",
        },
      ],
    };
  },
};
</script>

<template>
  <div class="categories">
    <h3>Customer Favorites</h3>
    <h4>Popular Catagories</h4>
    <div class="cards container">
      <div class="row">
        <category-card
          v-for="category in categories"
          :key="category.id"
          :category="category"
        />
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.categories {
  padding-top: 160px;

  h3 {
    color: #ff6868;
    font-family: Inter;
    font-size: 20px;
    font-style: normal;
    font-weight: 700;
    line-height: normal;
    letter-spacing: 3.5px;
    text-transform: uppercase;
    text-align: center;
  }

  h4 {
    color: #000;
    text-align: center;
    font-family: Inter;
    font-size: 60px;
    font-style: normal;
    font-weight: 700;
    line-height: normal;
  }

  .cards {
    padding: 0;
    .row {
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 30px;
    }
  }
}
</style>
