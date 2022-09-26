<template>
  <footer>
    <section class="d-flex container">
      <!-- DC COMICS LINKS -->
      <div class="me-5 mt-3">
        <h3 class="mt-3 pb-2">DC COMICS</h3>
        <ul>
          <li v-for="(item, index) in dcComicsLinks" :key="index">
            <p>{{ item.text }}</p>
          </li>
        </ul>
        <!-- SHOP LINKS -->
        <h3 class="mt-3 pb-2">SHOP</h3>
        <ul>
          <li v-for="(item, index) in shopLinks" :key="index">
            <p>{{ item.text }}</p>
          </li>
        </ul>
      </div>
      <!-- DC LINKS -->
      <div  class="me-5 mt-3">
        <h3 class="mt-3 pb-2">DC</h3>
        <ul>
          <li v-for="(item, index) in dcLinks" :key="index">
            <p>{{ item.text }}</p>
          </li>
        </ul>
      </div>
      <!-- SITES LINKS -->
      <div class="mt-3">
        <h3 class="mt-3 pb-2">SITES</h3>
        <ul>
          <li v-for="(item, index) in sitesLinks" :key="index">
            <p>{{ item.text }}</p>
          </li>
        </ul>
      </div>
      <div class="d-flex">
        <img src="../assets/dc-logo-bg.png" alt="dc-logo-bg">
      </div>
    </section>
  </footer>
</template>

<script>
export default {
    name: 'FooterSection',
    data: function () {
    return {
      dcComicsLinks: [
        {
          text: "Characters",
          active: false,
        },
        {
          text: "Comics",
          active: false,
        },
        {
          text: "Movies",
          active: false,
        },
        {
          text: "Tv",
          active: false,
        },
        {
          text: "Games",
          active: false,
        },
        {
          text: "Videos",
          active: false,
        },
        {
          text: "News",
          active: false,
        },
      ],
      shopLinks: [
        {
          text: "Shop DC",
          active: false,
        },
        {
          text: "Shop DC Collectibles",
          active: false,
        },
      ],
      dcLinks: [
        {
          text: "Terms Of Use",
          active: false,
        },
        {
          text: "Privacy policy (New)",
          active: false,
        },
        {
          text: "Ad Choices",
          active: false,
        },
        {
          text: "Advertising",
          active: false,
        },
        {
          text: "Jobs",
          active: false,
        },
        {
          text: "Subscription",
          active: false,
        },
        {
          text: "Talent Workshops",
          active: false,
        },
        {
          text: "CPSC Certificates",
          active: false,
        },
        {
          text: "Ratings",
          active: false,
        },
        {
          text: "Shop Help",
          active: false,
        },
        {
          text: "Contact Us",
          active: false,
        },
      ],
      sitesLinks: [
        {
          text: "DC",
          active: false,
        },
        {
          text: "Mad Magazines",
          active: false,
        },
        {
          text: "DC Kids",
          active: false,
        },
        {
          text: "DC Universe",
          active: false,
        },
        {
          text: "DC Power Visa",
          active: false,
        },
      ],
    };
  },
}
</script>

<style lang="scss" scoped>

  footer {
    height: 400px;
    background-image: url(../assets/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    position: relative;

    section {

        h3 {
        color: white;
        }
  
        ul {
          list-style: none;
          padding: 0;
          line-height: 10px;
  
          li {
            color: grey;
            font-weight: 500;
          }

        }

        img {
          position: absolute;
          bottom: -60px;
          right: 300px;
          overflow: hidden;     
          z-index: 0;
         }

      }
    }

</style>