<script>
export default {
  name: "TestimonialsVue",
};
</script>

<template>
  <div class="testimonials container">
    <div class="left-side">
      <span class="emoji emoji-face">😋</span>
      <span class="emoji emoji-pizza">🍕</span>
      <div class="testimonials-image">
        <img
          src="https://s3-alpha-sig.figma.com/img/ef0d/1d48/7273c3ffd4bc7fb0614dbba194a41031?Expires=1694390400&Signature=pQo5QFDkpvTB6zamtFSyyWykRT3~Fx8BfkYj0gVsno0HMmED~78nguRtMQY9Vc0EJKuxDIPI2bGPmlV3wmyTxtauuTH0TZ8g2lt72JxCNpvaakCjRT6zufWoGJ42vuYu1bK0KfkZDJVXVAFOPkUiw2oyqFcglUfW-NglNGc~rS0w3hcBWV1FsVpOef-OUftlRpeFKBLfHAYFAcafIWmVtqNk9hDmVQR8paEYlJixovI4~wgsI7KdFrNGaPhGWvRiD9IjIyypMEyA5zOD0qxyaxpH2LACcE9mLcj2ENfZYlMVFxVI7VoG95-dAZPGIdfMYHNJMa6jBSR5HItFQVMchQ__&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4"
          alt="testimonials"
        />
        <span>
          <span> Our Best Chef 😁 </span>
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="316"
            height="157"
            viewBox="0 0 316 157"
            fill="none"
          >
            <g filter="url(#filter0_d_1_183)">
              <path
                d="M37.2206 34.7879C37.5143 29.5925 43.8874 27.2774 47.4471 31.073C47.814 31.4642 48.2324 31.8038 48.6907 32.0823L53.4911 34.9992C60.8554 39.474 69.3072 41.8405 77.9245 41.8405H93.5H151H236.92C252.981 41.8405 266 54.8599 266 70.9202C266 86.9806 252.981 100 236.92 100H65.0798C49.0195 100 36 86.9806 36 70.9202V56.3804L37.2206 34.7879Z"
                fill="white"
              />
            </g>
            <defs>
              <filter
                id="filter0_d_1_183"
                x="0"
                y="0.193726"
                width="316"
                height="156.806"
                filterUnits="userSpaceOnUse"
                color-interpolation-filters="sRGB"
              >
                <feFlood flood-opacity="0" result="BackgroundImageFix" />
                <feColorMatrix
                  in="SourceAlpha"
                  type="matrix"
                  values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                  result="hardAlpha"
                />
                <feOffset dx="7" dy="14" />
                <feGaussianBlur stdDeviation="21.5" />
                <feComposite in2="hardAlpha" operator="out" />
                <feColorMatrix
                  type="matrix"
                  values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.14 0"
                />
                <feBlend
                  mode="normal"
                  in2="BackgroundImageFix"
                  result="effect1_dropShadow_1_183"
                />
                <feBlend
                  mode="normal"
                  in="SourceGraphic"
                  in2="effect1_dropShadow_1_183"
                  result="shape"
                />
              </filter>
            </defs>
          </svg>
        </span>
      </div>
    </div>
    <div class="right-side">
      <div class="header-container">
        <p class="header">Testimonials</p>
        <p class="testimonials-saying">What Our Customers Say About Us</p>
        <p class="quote">
          “I had the pleasure of dining at Foodi last night, and I'm still
          raving about the experience! The attention to detail in presentation
          and service was impeccable”
        </p>
      </div>
      <div class="footer-container">
        <div class="right">
          <div class="footer-image">
            <img class="img-1" src="@/assets/img/testimonials_1.png" alt="" />
            <img src="@/assets/img/testimonials_2.png" alt="" />
            <img src="@/assets/img/testimonials_3.png" alt="" />
          </div>
        </div>
        <div class="left">
          <p class="footer-header">Customer Feedback</p>
          <div class="rating-container">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="24"
              height="24"
              viewBox="0 0 24 24"
              fill="none"
            >
              <g clip-path="url(#clip0_1_69)">
                <path
                  d="M1.3268 12.4003L4.8868 15.0003L3.5348 19.1873C3.31631 19.8367 3.31354 20.5393 3.52691 21.1904C3.74027 21.8415 4.15834 22.4062 4.7188 22.8003C5.26965 23.2071 5.93719 23.425 6.62195 23.4216C7.30671 23.4182 7.97204 23.1936 8.5188 22.7813L11.9998 20.2193L15.4818 22.7783C16.0317 23.1828 16.6956 23.4025 17.3782 23.4058C18.0607 23.4091 18.7268 23.1959 19.2806 22.7968C19.8343 22.3978 20.2473 21.8334 20.4601 21.1848C20.6729 20.5362 20.6745 19.8369 20.4648 19.1873L19.1128 15.0003L22.6728 12.4003C23.2219 11.9988 23.6302 11.4341 23.8391 10.7867C24.0481 10.1394 24.0472 9.44251 23.8365 8.79571C23.6258 8.14891 23.216 7.58525 22.6658 7.18523C22.1156 6.7852 21.4531 6.56929 20.7728 6.56832H16.3998L15.0728 2.43232C14.8641 1.78128 14.4541 1.21333 13.9018 0.810386C13.3495 0.407437 12.6835 0.190308 11.9998 0.190308C11.3161 0.190308 10.6501 0.407437 10.0978 0.810386C9.54553 1.21333 9.13548 1.78128 8.9268 2.43232L7.5998 6.56832H3.2308C2.55054 6.56929 1.88799 6.7852 1.33778 7.18523C0.787564 7.58525 0.377837 8.14891 0.167118 8.79571C-0.0436018 9.44251 -0.0445344 10.1394 0.164453 10.7867C0.37344 11.4341 0.781657 11.9988 1.3308 12.4003H1.3268Z"
                  fill="#FFE605"
                />
              </g>
              <defs>
                <clipPath id="clip0_1_69">
                  <rect width="24" height="24" fill="white" />
                </clipPath>
              </defs>
            </svg>
            <span class="rating"> 4.9</span>
            <span class="review"> (18.6k Reviews) </span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.testimonials {
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 240px;

  .left-side {
    position: relative;
    display: flex;
    justify-content: space-between;
    align-items: center;

    &::before {
      content: "";
      width: 100%;
      height: 50%;
      background-color: #53ec62;
      position: absolute;
      bottom: 5px;
      border-radius: 150px 150px 50px 50px;
      z-index: -1;
    }
    .emoji {
      font-size: 40px;
      position: absolute;
    }

    .emoji-face {
      transform: rotate(-17.029deg);
      bottom: 30%;
      left: -30px;
    }

    .emoji-pizza {
      transform: rotate(80.994deg);
      bottom: 30%;
      right: -30px;
    }

    .testimonials-image {
      width: 100%;
      height: 100%;
      position: relative;

      img {
        max-width: 506px;
        max-height: 744px;
      }

      span {
        position: absolute;
        bottom: -60px;
        right: -90px;

        span {
          color: #202020;
          font-family: Inter;
          font-size: 20px;
          font-style: normal;
          font-weight: 600;
          line-height: normal;
          position: absolute;
          display: flex;
          justify-content: center;
          align-items: center;
          top: -50%;
          left: 0%;
          transform: translate(-10%, 0%);
        }
      }
    }
  }

  .right-side {
    .header-container {
      .header {
        color: #ff6868;
        font-family: Inter;
        font-size: 20px;
        font-style: normal;
        font-weight: 700;
        line-height: normal;
        letter-spacing: 3.5px;
        text-transform: uppercase;
      }

      .testimonials-saying {
        width: 635px;
        color: #000;
        font-family: Inter;
        font-size: 60px;
        font-style: normal;
        font-weight: 700;
        line-height: 131.023%;
      }

      .quote {
        color: #555;
        font-family: Inter;
        font-size: 26px;
        font-style: normal;
        font-weight: 500;
        line-height: 159%;
      }
    }

    .footer-container {
      display: flex;
      justify-content: center;
      align-items: center;
      gap: 40px;

      .right {
        padding-top: 30px;

        .footer-image {
          display: flex;
          justify-content: start;
          align-items: center;
          width: fit-content;

          img {
            border: 6px solid #fff;
            border-radius: 50%;
            margin-right: -15px;

            &:first-of-type {
              z-index: -1;
              background-color: #ffe8ad;
            }

            &:last-of-type {
              margin: -15px;
            }
          }
        }
      }

      .left {
        .footer-header {
          color: #000;
          font-family: Inter;
          font-size: 26px;
          font-style: normal;
          font-weight: 600;
          line-height: normal;
        }

        .rating-container {
          display: flex;
          justify-content: center;
          align-items: center;
          gap: 10px;

          .review {
            color: #807e7e;
            font-family: Inter;
            font-size: 24px;
            font-style: normal;
            font-weight: 500;
            line-height: normal;
          }

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
}
</style>
