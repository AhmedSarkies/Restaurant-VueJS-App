<script>
export default {
  name: "LandingHeroVue",
};
</script>

<template>
  <div class="container">
    <div class="row d-flex">
      <div class="left-side col-lg-6 col-md-8 col-sm-12">
        <div class="top">
          <h1>
            Dive into Delights <br />
            Of Delectable <span>Food</span>
          </h1>
        </div>
        <div class="center">
          <h2>
            Where Each Plate Weaves a Story of Culinary Mastery and Passionate
            Craftsmanship
          </h2>
        </div>
        <div class="bottom">
          <button>Order Now</button>
          <div class="watch-video">Watch Video</div>
          <div class="play-video">
            <img src="@/assets/img/polygon.svg" />
          </div>
        </div>
      </div>
      <div class="right-side col-lg-6 col-md-8 col-sm-12">
        <div class="hero">
          <span>Hot spicy Food 🌶</span>
          <img src="@/assets/img/hero3.png" alt="" />
        </div>
        <div class="cards">
          <div class="card">
            <div class="card-image">
              <img src="@/assets/img/card-1.png" alt="" />
            </div>
            <div class="card-body">
              <p class="card-title">Spicy noodles</p>
              <div class="starts">
                <img src="../assets/img/fi-sr-star.svg" alt="" />
                <img src="../assets/img/fi-sr-star.svg" alt="" />
                <img src="../assets/img/fi-sr-star.svg" alt="" />
                <img src="../assets/img/fi-br-star.svg" alt="" />
                <img src="../assets/img/fi-br-star.svg" alt="" />
              </div>
              <p class="price"><span>$</span>18.00</p>
            </div>
          </div>
          <div class="card">
            <div class="card-image">
              <img src="@/assets/img/card-2.png" alt="" />
            </div>
            <div class="card-body">
              <p class="card-title">Vegetarian salad</p>
              <div class="starts">
                <img src="../assets/img/fi-sr-star.svg" alt="" />
                <img src="../assets/img/fi-sr-star.svg" alt="" />
                <img src="../assets/img/fi-sr-star.svg" alt="" />
                <img src="../assets/img/fi-sr-star.svg" alt="" />
                <img src="../assets/img/fi-br-star.svg" alt="" />
              </div>
              <p class="price"><span>$</span>23.00</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.left-side {
  .top {
    padding-top: 75px;
    h1 {
      color: #000;
      font-family: Inter;
      font-size: 62px;
      font-style: normal;
      font-weight: 800;
      line-height: 145.523%;

      span {
        color: #39db4a;
      }
    }
  }

  .center {
    margin: 60px 0;
    h2 {
      color: #4a4a4a;
      font-family: Inter;
      font-size: 26px;
      font-style: normal;
      font-weight: 500;
      line-height: 170.5%;
    }
  }

  .bottom {
    display: flex;
    justify-content: space-between;
    align-items: center;

    button {
      border-radius: 40px;
      background: #39db4a;
      box-shadow: -2px 22px 38px 0px rgba(142, 255, 154, 0.5);
      border: none;
      padding: 15px 30px;
      color: #fff;
      font-family: Inter;
      font-size: 26px;
      font-style: normal;
      font-weight: 600;
      line-height: normal;
      cursor: pointer;
    }

    .watch-video {
      color: #4d4d4d;
      font-family: Inter;
      font-size: 26px;
      font-style: normal;
      font-weight: 600;
      line-height: normal;
    }

    .play-video {
      box-shadow: 6px 27px 34px rgba(0, 0, 0, 0.1);
      width: 80px;
      height: 80px;
      border-radius: 50%;
      display: flex;
      justify-content: center;
      align-items: center;
      cursor: pointer;
      margin-right: 100px;
    }
  }
}

.right-side {
  display: flex;
  justify-content: center;
  align-items: end;
  position: relative;

  .hero {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    height: 100%;

    img {
      width: 100%;
      border-radius: 115% 93% 96% 3%/88% 75% 130% 0%;
      position: absolute;
      right: -10px;
      bottom: 31px;
    }

    &::before {
      content: "";
      width: 90%;
      height: 90%;
      border-radius: 50%;
      background-color: #39db4a;
    }

    & span {
      position: absolute;
      color: #ff6868;
      font-family: Inter;
      font-size: 20px;
      font-style: normal;
      font-weight: 600;
      line-height: normal;
      background-color: #fbfbfb;
      padding: 10px 30px;
      border-radius: 20px 20px 0 20px;
      box-shadow: 26px 22px 51px rgba(0, 0, 0, 0.14);
      top: 7%;
      left: -10%;

      &::after {
        content: "";
        position: absolute;
        width: 30px;
        height: 30px;
        border: 10px solid;
        border-color: #fbfbfb transparent transparent #fbfbfb;
        bottom: -7px;
        right: -8px;
        border-radius: 10% 225% 0% 115%/10% 200% 0% 225%;
        transform: rotate(190deg);
      }
    }
  }

  .cards {
    display: flex;
    justify-content: center;
    align-items: center;
    position: absolute;
    gap: 20px;
    bottom: -8%;

    .card {
      display: flex;
      justify-content: center;
      align-items: center;
      width: 100%;
      height: 100%;
      background-color: #fff;
      box-shadow: 7px 35px 51px 0px rgba(0, 0, 0, 0.14);
      border-radius: 25px;
      padding: 10px 50px 10px 15px;
      gap: 15px;

      .card-image {
        margin: 0;
        padding: 0;
        display: flex;
        justify-content: center;
        align-items: center;
        border-radius: 25px;
        overflow: hidden;
      }

      .card-body {
        .card-title {
          margin: 0;
          color: #2c2c2c;
          font-family: Inter;
          font-size: 22px;
          font-style: normal;
          font-weight: 600;
          line-height: normal;
          width: 150%;
        }

        .starts {
          display: flex;
          justify-content: start;
          align-items: center;
          margin: 0;
          gap: 5px;
        }

        .price {
          color: #515151;
          font-family: Inter;
          font-size: 24px;
          font-style: normal;
          font-weight: 600;
          line-height: normal;
          margin: 0;

          & span {
            color: #ff7979;
          }
        }
      }
    }
  }
}
</style>
