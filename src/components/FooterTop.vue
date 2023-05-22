<script>
export default {
  name: "FooterTop",
  data() {
    return {
      menuLeft: [
        {
          title: "DC Comics",
          items: [
            "Characters",
            "Comics",
            "Movies",
            "TV",
            "Games",
            "Videos",
            "News",
          ],
        },
        {
          title: "Shop",
          items: ["Shop DC", "Shop DC Collectibles"],
        },
      ],
      menuRight: [
        {
          title: "DC",
          items: [
            "Terms of Use",
            "Privacy Policy (New)",
            "Ad Choice",
            "Avertising",
            "Jobs",
            "Subscriptions",
            "Talent Workshop",
            "CPSC Certificates",
            "Ratings",
            "Shop Help",
            "Contact Us",
          ],
        },
        {
          title: "Sites",
          items: [
            "DC",
            "MAD Magazine",
            "DC Kids",
            "DC Universe",
            "DC Power Visa",
          ],
        },
      ],
    };
  },
};
</script>
<template>
  <div class="footer_top">
    <div class="top_container">
      <div class="footer_menu">
        <div class="my_col">
          <div class="my_row pb-4" v-for="list in menuLeft">
            <h5>{{ list.title.toUpperCase() }}</h5>
            <ul class="list-unstyled flex-column">
              <li v-for="item in list.items">
                <a href="#">{{ item }}</a>
              </li>
            </ul>
          </div>
        </div>
        <div class="my_col" v-for="list in menuRight">
          <h5>{{ list.title.toUpperCase() }}</h5>
          <ul class="list-unstyled">
            <li v-for="item in list.items">
              <a href="#">{{ item }}</a>
            </li>
          </ul>
        </div>
      </div>
      <div class="footer_logo"></div>
    </div>
  </div>
</template>

<style lang="scss" scoped></style>