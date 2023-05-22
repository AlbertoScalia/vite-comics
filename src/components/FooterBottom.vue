<script>
export default {
  name: "FooterBottom",
  data() {
    return {
      socials: [
        {
          name: "Facebook",
          img: "/img/footer-facebook.png",
        },
        {
          name: "Twitter",
          img: "/img/footer-twitter.png",
        },
        {
          name: "YouTube",
          img: "/img/footer-youtube.png",
        },
        {
          name: "Pinterest",
          img: "/img/footer-pinterest.png",
        },
        {
          name: "Periscope",
          img: "/img/footer-periscope.png",
        },
      ],
    };
  },
};
</script>
<template>
  <div class="footer_bottom">
      <div class="bottom_container">
        <div class="bottom_left">
            <button type="button" class="btn btn-outline-primary">SIGN-UP NOW!</button>
        </div>
        <div class="bottom_right d-flex">
            <span>FOLLOW US</span>
            <ul class="list-unstyled d-flex mb-0">
                <li v-for="social in socials">
                    <a href="#">
                        <img :src="social.img" :alt="social.name">
                    </a>
                </li>
            </ul>
        </div>
      </div>
    </div>
</template>

<style lang="scss" scoped></style>
