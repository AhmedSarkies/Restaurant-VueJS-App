<script>
export default {
  name: "HeaderVue",
  data: () => {
    return {
      isOpen: false,
    };
  },
  methods: {
    isOpenFn: function () {
      this.isOpen = !this.isOpen;
    },
  },
};
</script>

<template>
  <div class="container">
    <div class="row">
      <div class="logo-container left col-xxl-1 col-xl-2 col-lg-3 col-md-4">
        <span class="layout">
          <img class="logo logo-f" src="@/assets/img/F.svg" alt="" />
        </span>
        <img class="logo logo-oodi" src="@/assets/img/oodi.svg" alt="" />
      </div>
      <div :class="`menu-icon ${isOpen && 'open'}`" @click="isOpenFn">
        <span></span>
        <span></span>
        <span></span>
      </div>
      <div class="menu col-xxl-8 col-xl-10 col-lg-9">
        <ul class="center col-xl-12 col-xxl-12 col-lg-8 col-sm-12">
          <li class="active">Home</li>
          <li>Menu <img src="@/assets/img/group.svg" /></li>
          <li>Services <img src="@/assets/img/group.svg" /></li>
          <li>Offers</li>
        </ul>
        <div class="right col-lg-4 col-md-3 col-sm-12">
          <div class="icons">
            <img
              class="search-icon"
              src="@/assets/img/icon_search.svg"
              alt=""
            />
            <div class="shopping-bag">
              <img src="@/assets/img/fi-rr-shopping-bag.svg" alt="" />
              <span>0</span>
            </div>
          </div>
          <div class="contact">
            <img src="@/assets/img/fi-rr-phone-call.svg" alt="" />
            Contact
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.row {
  justify-content: space-between;
  align-items: center;
  margin-bottom: 80px;

  .layout {
    display: inline-flex;
    border-radius: 8px;
    background-color: #39db4a;
    width: 34px;
    height: 41px;
    justify-content: center;
    align-items: center;
    margin-right: 5px;
  }

  .center,
  .right {
    display: flex;
    align-items: center;
    font-family: Poppins;
    font-size: 20px;
    font-style: normal;
    font-weight: 500;
    line-height: normal;
    padding: 0;
  }

  .left {
    padding: 0;

    @media (max-width: 992px) {
      .layout {
        width: 25px;
        height: 35px;

        .logo-f {
          width: 15px;
        }
      }

      .logo-oodi {
        width: 50px;
      }
    }
  }

  .right {
    align-items: center;
    gap: 25px;

    .icons {
      display: flex;
      justify-content: center;
      align-items: center;
      gap: 30px;
    }
  }

  .menu-icon {
    display: none;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
    position: relative;
    width: 64px;
    height: 45px;
    gap: 5px;
    background-color: #39db4a;
    padding: 10px 7px;
    border: 2px solid #5f8262;
    border-radius: 5px;
    cursor: pointer;

    @media (max-width: 992px) {
      display: flex;
    }

    span {
      display: block;
      width: 45px;
      height: 5px;
      border-radius: 5px;
      background-color: #fff;
      opacity: 1;
      transition: all 0.5s ease-in-out;
    }

    &.open {
      justify-content: center;

      span {
        position: absolute;
        transform-origin: center;
        transition: all 0.5s ease-in-out;

        &:nth-of-type(2) {
          opacity: 0;
        }

        &:first-of-type {
          transform: translateY(0) rotate(45deg);
        }
        &:last-of-type {
          transform: translateY(0) rotate(-45deg);
        }
      }
    }
  }

  .open + .menu {
    @media (max-width: 992px) {
      opacity: 1;
      right: 0;
      top: 70px;
      padding: 20px;
      background-color: #fff;
      width: 50%;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      transition: all 0.5s ease-in-out;
    }

    @media (max-width: 767px) {
      width: 75%;
    }
    @media (max-width: 567px) {
      width: 100%;
    }
  }

  .menu {
    display: flex;
    justify-content: space-between;
    align-items: center;

    @media (max-width: 992px) {
      flex-direction: column;
      position: absolute;
      opacity: 0;
      width: 50%;
      top: 70px;
      right: -100%;
      z-index: 99999999999;
      transition: all 0.5s ease-in-out;

      .right {
        padding: 30px 0;
      }

      .center,
      .right {
        flex-direction: column;
        align-items: center;
        direction: rtl;
        gap: 30px;

        .icons {
          display: flex;
          justify-content: center;
          align-items: center;
          padding-top: 10px;
          gap: 30px;
        }

        .contact {
          direction: ltr;
        }
      }
    }

    @media (max-width: 767px) {
      width: 75%;
    }
    @media (max-width: 567px) {
      width: 100%;
    }

    .center {
      justify-content: center;
      gap: 60px;

      @media (max-width: 1200px) {
        gap: 50px;
      }

      @media (max-width: 992px) {
        gap: 30px;
      }

      li {
        cursor: pointer;
        &:hover {
          color: #39db4a;
          transition: all 0.2s;
        }

        &.active {
          color: #39db4a;
        }
      }
    }

    .right {
      justify-content: space-around;

      .search-icon {
        cursor: pointer;
      }

      .shopping-bag {
        position: relative;
        cursor: pointer;

        span {
          position: absolute;
          display: flex;
          justify-content: center;
          align-items: center;
          top: -10px;
          right: -10px;
          background-color: #39db4a;
          color: #fff;
          font-family: Inter;
          font-size: 14px;
          font-style: normal;
          font-weight: 700;
          line-height: normal;
          border-radius: 50%;
          width: 20px;
          height: 20px;
        }
      }

      .contact {
        background-color: #39db4a;
        border-radius: 40px;
        padding: 10px 25px;
        display: flex;
        justify-content: center;
        align-items: center;
        color: #fff;
        font-family: Poppins;
        font-size: 20px;
        font-style: normal;
        font-weight: 500;
        line-height: normal;
        cursor: pointer;

        img {
          margin-right: 5px;
        }
      }
    }
  }
}
</style>
