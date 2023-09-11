<script>
import DishesCard from "./DishesCard.vue";
export default {
  name: "SpecialDishes",
  components: { DishesCard },
  data: () => {
    return {
      cards: [
        {
          id: 1,
          title: "Fattoush salad",
          desc: "Description of the item",
          price: 24,
          rating: 4.9,
          fav: true,
          img: "https://s3-alpha-sig.figma.com/img/c63c/1ab0/6b87da252d0637f480fe9e0485c5a3ef?Expires=1694390400&Signature=YchwAF6A3alQUzbhb9oJv5SlJQH52PtPNTqs5o44hzIFTGm7rn6-Fwv~nsT9S01Arv-s0w8by0N8v7gayue~RuqJ~haQ2DQLCTXwKcyXGpzu2O~QewxO6aLhW1LV1Fi02YpNAy0zhHpaDQEohOTQ7bIkCObcvE6gDibSjl6T5YcgBXSYsTpDN6WP-LXeiNIqY8COckjap-fsfK4nRj2JcDcAD-yuWclAKHf6upTYo5gC5A1DK~-812Kre-KD0y43Zs3~Tp~rczBu6P3XrDvX0GLYttF9NGPVQsugo4cGT5254FnRkisP5MpWcFyze1Li0TGPHrviiKMB4rXwQqJOxQ__&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4",
        },
        {
          id: 2,
          title: "Vegetable salad",
          desc: "Description of the item",
          price: 22,
          rating: 4.6,
          fav: false,
          img: "https://s3-alpha-sig.figma.com/img/6701/42ad/7e70ee8eec6a4308bddb455ca1200e6d?Expires=1694390400&Signature=Dut246Qto0KUaCYLJIJ27UkNRcTc54dFQ34d~Xl9FonYORL2uWv~zc6N8bpcCV6OCX0b5sa3CMvOqLAjnW6Q~g8q-OVRZ2Dvtmva9YoKpwDL-Xavr9hZ0gP~dAf9-TqJVwI7XG~BWORp~eWral2ppf4hr0os2xOH9rX2PkNLhs6YdtK-E3qi8Q1Y-JMAr0aV464oNnaOdODSGIH4fJ-KsVMRS5cm7nkID5dfuukEzQXRuJaccq3YdSqZPzWiA7ggPJhPjmptity8xolLMmmFS1-UhxjlzxZlfAXgYylpJFkVIAPIQZ6TF3CHxtwJ6k1tdyUxYoRIRLjWGDDF6pUTMA__&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4",
        },
        {
          id: 3,
          title: "Egg vegi salad",
          desc: "Description of the item",
          price: 23,
          rating: 4.5,
          fav: false,
          img: "https://s3-alpha-sig.figma.com/img/e5f6/6399/92cb147d6be498d52028200fb734a790?Expires=1694390400&Signature=dL1MEC7XuWUtNJ6SvyZVMORe1XB~y3dlkpIVgAibkwPlZbmjozhI7xPBAYG-98PApcvMTRaCjanlytu9AyKo-S9-VatYFRl0DgcL89AgHrDqA0UtJYy4GKMgq5GHi8dB1HnlOp8neusd2Ly-I1ZqlE7RAPPtGKREdVYxCPYbgM1aJTw6Fo0icQcGP6IwqxrSsr6OC5te97H4OuaY-MEEiIm8HPN4GUvrJrnJrtrIoMZzimBWHvMS8AfUMuWoArGXBSgIQOCHaL9gNThh~Kjmo-7SHnKUAKWEBnrQWnvcpmMSysz5vEqAannMQURPvL~Np4kzV0McPcfiVKRKv35Ftg__&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4",
        },
      ],
    };
  },
};
</script>

<template>
  <div class="container">
    <div class="container-header">
      <p class="special-dishes">Special Dishes</p>
      <div class="container-header-body">
        <p class="standout-dishes-from">Standout Dishes From Our Menu</p>
        <div class="actions">
          <button class="prev">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="12"
              height="20"
              viewBox="0 0 12 20"
              fill="none"
            >
              <path
                d="M9.76453 2L2.00003 9.7645"
                stroke="#6F6E6E"
                stroke-width="4"
                stroke-linecap="round"
              />
              <path
                d="M9.76453 18L2.00003 10.2355"
                stroke="#6F6E6E"
                stroke-width="4"
                stroke-linecap="round"
              />
            </svg>
          </button>
          <button class="next">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="12"
              height="20"
              viewBox="0 0 12 20"
              fill="none"
            >
              <path
                d="M9.76453 2L2.00003 9.7645"
                stroke-width="4"
                stroke-linecap="round"
              />
              <path
                d="M9.76453 18L2.00003 10.2355"
                stroke-width="4"
                stroke-linecap="round"
              />
            </svg>
          </button>
        </div>
      </div>
    </div>
    <div class="container-body">
      <div class="row">
        <dishes-card v-for="card in cards" :key="card.id" :card="card" />
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.container {
  padding-top: 160px;

  .container-header {
    display: flex;
    flex-direction: column;
    justify-content: center;

    .special-dishes {
      color: #ff6868;
      font-family: Inter;
      font-size: 20px;
      font-style: normal;
      font-weight: 700;
      line-height: normal;
      letter-spacing: 3.5px;
      text-transform: uppercase;
    }

    .container-header-body {
      display: flex;
      justify-content: space-between;
      align-items: center;

      .standout-dishes-from {
        color: #000;
        font-family: Inter;
        font-size: 60px;
        font-style: normal;
        font-weight: 700;
        line-height: 131.523%;
        width: 580px;
        padding-top: 25px;
        margin-top: 0;
      }

      .actions {
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 30px;

        button {
          display: flex;
          justify-content: center;
          align-items: center;
          width: 80px;
          height: 80px;
          border: none;
          border-radius: 50%;
          opacity: 1;
          cursor: pointer;
          transition: opacity 0.2s ease-in-out;

          &:hover {
            opacity: 0.8;
            transition: opacity 0.2s ease-in-out;
          }

          &.prev {
            background-color: #efefef;
          }

          &.next {
            background-color: #39db4a;

            & svg {
              stroke: #fff;
              transform: rotate(180deg);
            }
          }
        }
      }
    }
  }

  .container-body {
    .row {
      gap: 50px;
    }
  }
}
</style>
