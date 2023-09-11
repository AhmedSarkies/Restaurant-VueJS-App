<template>
  <div class="card col-lg-3 col-md-6 col-sm-12">
    <span class="fav">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        width="24"
        height="24"
        viewBox="0 0 24 24"
        fill="none"
        v-if="card.fav"
      >
        <g clip-path="url(#clip0_1_105)">
          <path
            d="M17.5 1.91653C16.3739 1.93405 15.2724 2.24839 14.3068 2.82781C13.3411 3.40722 12.5453 4.2312 12 5.21653C11.4546 4.2312 10.6589 3.40722 9.69323 2.82781C8.72753 2.24839 7.62604 1.93405 6.49999 1.91653C4.70493 1.99453 3.01369 2.77979 1.79577 4.10077C0.577848 5.42175 -0.0677617 7.17106 -1.11917e-05 8.96653C-1.11917e-05 13.5135 4.78599 18.4795 8.79999 21.8465C9.69621 22.5997 10.8293 23.0126 12 23.0126C13.1706 23.0126 14.3038 22.5997 15.2 21.8465C19.214 18.4795 24 13.5135 24 8.96653C24.0677 7.17106 23.4221 5.42175 22.2042 4.10077C20.9863 2.77979 19.295 1.99453 17.5 1.91653Z"
            fill="white"
          />
        </g>
        <defs>
          <clipPath id="clip0_1_105">
            <rect width="24" height="24" fill="white" />
          </clipPath>
        </defs>
      </svg>
      <svg
        xmlns="http://www.w3.org/2000/svg"
        width="24"
        height="24"
        viewBox="0 0 24 24"
        fill="none"
        v-else
      >
        <g clip-path="url(#clip0_1_103)">
          <path
            d="M17.25 1.85071C16.2243 1.86063 15.2152 2.11065 14.3035 2.58073C13.3918 3.05081 12.6029 3.72788 12 4.55771C11.397 3.72788 10.6081 3.05081 9.69644 2.58073C8.78476 2.11065 7.77565 1.86063 6.74996 1.85071C4.89173 1.92491 3.13848 2.73189 1.87358 4.09517C0.608672 5.45846 -0.0649657 7.26713 -4.03235e-05 9.12571C-4.03235e-05 13.6777 4.67396 18.5507 8.59996 21.8377C9.55329 22.6393 10.7589 23.0788 12.0045 23.0788C13.25 23.0788 14.4556 22.6393 15.409 21.8377C19.331 18.5507 24.009 13.6777 24.009 9.12571C24.0738 7.26563 23.399 5.45564 22.1322 4.0921C20.8653 2.72856 19.1098 1.9226 17.25 1.85071ZM13.477 19.5387C13.0634 19.8869 12.5401 20.0779 11.9995 20.0779C11.4588 20.0779 10.9355 19.8869 10.522 19.5387C5.74196 15.5307 2.99996 11.7357 2.99996 9.12571C2.9362 8.06292 3.29424 7.01789 3.99634 6.21749C4.69844 5.4171 5.68793 4.92596 6.74996 4.85071C7.81199 4.92596 8.80148 5.4171 9.50358 6.21749C10.2057 7.01789 10.5637 8.06292 10.5 9.12571C10.5 9.52353 10.658 9.90506 10.9393 10.1864C11.2206 10.4677 11.6021 10.6257 12 10.6257C12.3978 10.6257 12.7793 10.4677 13.0606 10.1864C13.3419 9.90506 13.5 9.52353 13.5 9.12571C13.4362 8.06292 13.7942 7.01789 14.4963 6.21749C15.1984 5.4171 16.1879 4.92596 17.25 4.85071C18.312 4.92596 19.3015 5.4171 20.0036 6.21749C20.7057 7.01789 21.0637 8.06292 21 9.12571C21 11.7357 18.258 15.5307 13.477 19.5387Z"
            fill="white"
          />
        </g>
        <defs>
          <clipPath id="clip0_1_103">
            <rect width="24" height="24" fill="white" />
          </clipPath>
        </defs>
      </svg>
    </span>
    <div class="header">
      <img :src="card.img" :alt="card.title" />
    </div>
    <div class="body">
      <p class="title">{{ card.title }}</p>
      <span class="desc">{{ card.desc }}</span>
      <div class="price-rating-container">
        <span class="price"
          ><span>$</span>{{ parseFloat(card.price).toFixed(2) }}</span
        >
        <div class="rating-container">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="24"
            height="24"
            viewBox="0 0 24 24"
            fill="none"
          >
            <g clip-path="url(#clip0_1_97)">
              <path
                d="M1.3268 12.4003L4.8868 15.0003L3.5348 19.1873C3.31631 19.8367 3.31354 20.5393 3.52691 21.1904C3.74027 21.8415 4.15834 22.4062 4.7188 22.8003C5.26965 23.2071 5.93719 23.425 6.62195 23.4216C7.30671 23.4182 7.97204 23.1936 8.5188 22.7813L11.9998 20.2193L15.4818 22.7783C16.0317 23.1828 16.6956 23.4024 17.3782 23.4058C18.0607 23.4091 18.7268 23.1959 19.2806 22.7968C19.8343 22.3977 20.2473 21.8333 20.4601 21.1848C20.6729 20.5362 20.6745 19.8369 20.4648 19.1873L19.1128 15.0003L22.6728 12.4003C23.2219 11.9988 23.6302 11.4341 23.8391 10.7867C24.0481 10.1393 24.0472 9.44249 23.8365 8.79569C23.6258 8.1489 23.216 7.58523 22.6658 7.18521C22.1156 6.78519 21.4531 6.56927 20.7728 6.56831H16.3998L15.0728 2.43231C14.8641 1.78126 14.4541 1.21332 13.9018 0.810371C13.3495 0.407422 12.6835 0.190292 11.9998 0.190292C11.3161 0.190292 10.6501 0.407422 10.0978 0.810371C9.54553 1.21332 9.13548 1.78126 8.9268 2.43231L7.5998 6.56831H3.2308C2.55054 6.56927 1.88799 6.78519 1.33778 7.18521C0.787564 7.58523 0.377837 8.1489 0.167118 8.79569C-0.0436018 9.44249 -0.0445344 10.1393 0.164453 10.7867C0.37344 11.4341 0.781657 11.9988 1.3308 12.4003H1.3268Z"
                fill="#FFE605"
              />
            </g>
            <defs>
              <clipPath id="clip0_1_97">
                <rect width="24" height="24" fill="white" />
              </clipPath>
            </defs>
          </svg>
          <span class="rating">{{ card.rating }}</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "DishesCard",
  props: ["card"],
};
</script>

<style lang="scss" scoped>
.card {
  border-radius: 40px;
  background-color: #fff;
  box-shadow: 2px 9px 42px 0px rgba(0, 0, 0, 0.08);
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 30px 50px;
  max-width: 446px;
  max-height: 523px;
  position: relative;

  & span.fav {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 87px;
    height: 75px;
    background-color: #39db4a;
    border-radius: 0px 37.5px 0px 42.5px;
    position: absolute;
    top: 0;
    right: 0;
  }

  .header {
    display: flex;
    justify-content: center;
    align-items: center;

    img {
      width: 276px;
      height: 276px;
    }
  }

  .body {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: start;
    width: 100%;
    padding-top: 30px;
    gap: 15px;

    .title {
      color: #000;
      font-family: Inter;
      font-size: 30px;
      font-style: normal;
      font-weight: 600;
      line-height: normal;
      margin: 0;
    }

    .desc {
      color: #555;
      font-family: Inter;
      font-size: 22px;
      font-style: normal;
      font-weight: 600;
      line-height: normal;
    }

    .price-rating-container {
      display: flex;
      justify-content: space-between;
      align-items: center;
      width: 100%;
      padding-top: 10px;

      .price {
        color: #000;
        font-family: Inter;
        font-size: 30px;
        font-style: normal;
        font-weight: 600;
        line-height: normal;

        span {
          color: #ff6868;
          font-family: Inter;
          font-size: 24px;
          font-style: normal;
          font-weight: 600;
          line-height: normal;
        }
      }

      .rating-container {
        display: flex;
        justify-content: center;
        align-items: center;

        svg {
          width: 24px;
          height: 24px;
        }

        .rating {
          color: #454545;
          font-family: Inter;
          font-size: 24px;
          font-style: normal;
          font-weight: 600;
          line-height: normal;
        }
      }
    }
  }
}
</style>
