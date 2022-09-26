<template>
  <section class="container">
    <ul class="d-flex justify-content-center">
      <li v-for="(item, index) in blueSectionArray" :key="index" class="d-flex justify-content-evenly p-4 align-items-center">
        <img :src="require(`../assets/imgBlue/${item.image}`)" :alt="item.text" class="img-fluid fl-blueicons">
        <p class="d-flex">{{ item.text }}</p>
      </li>
    </ul>
  </section>
</template>

<script>
export default {
    name: 'BlueMainSection',
    data: function () {
    return {
      blueSectionArray: [
        {
          image: "buy-comics-digital-comics.png",
          text: "Digital Comics",
        },
        {
          image: "buy-comics-merchandise.png",
          text: "DC Merchandise",
        },
        {
          image: "buy-comics-subscriptions.png",
          text: "Subscription",
        },
        {
          image: "buy-comics-shop-locator.png",
          text: "Comic Shop Locator",
        },
        {
          image: "buy-dc-power-visa.svg",
          text: "DC Power Visa",
        },
      ],
    };
  }
}
</script>

<style lang="scss" scoped>

  section {
    height: 120px;
    background-color: #0c7cec;
    min-width: 100%;
    z-index: 2;
    position: relative;

    ul{
      list-style: none;

      li {

        &:hover {
        cursor: pointer;
      }
      
      }
    }

    p {
      color: white;
      text-transform: uppercase;
      font-weight: 500;

    }

    .fl-blueicons {
      height: 70px;
      margin: 0px 10px;

    }

  }



</style>