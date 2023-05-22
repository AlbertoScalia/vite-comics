<script>
export default {
  name: "SiteFooter",
  data() {
    return {
       footerMenu: [
        {
            title: 'DC Comics',
            items: [
                'Characters',
                'Comics',
                'Movies',
                'TV',
                'Games',
                'Videos',
                'News'
            ]
        },
        {
            title: 'DC',
            items: [
                'Terms of Use',
                'Privacy Policy (New)',
                'Ad Choice',
                'Avertising',
                'Jobs',
                'Subscriptions',
                'Talent Workshop',
                'CPSC Certificates',
                'Ratings',
                'Shop Help',
                'Contact Us'
            ]
        },
        {
            title: 'Sites',
            items: [
                'DC',
                'MAD Magazine',
                'DC Kids',
                'DC Universe',
                'DC Power Visa'
            ]
        },
        {
            title: 'Shop',
            items: [
                'Shop DC',
                'Shop DC Collectibles'
            ] 
        }
    ],
    socials: [
        {
            name: 'Facebook',
            img: '/img/footer-facebook.png', 
        },
        {
            name: 'Twitter',
            img: '/img/footer-twitter.png', 
        },
        {
            name: 'YouTube',
            img: '/img/footer-youtube.png', 
        },
        {
            name: 'Pinterest',
            img: '/img/footer-pinterest.png', 
        },
        {
            name: 'Periscope',
            img: '/img/footer-periscope.png', 
        }
    ]
    }
    
  }
};
</script>

<template>
  <footer>
    <div class="footer_top">
      <div class="top_container">
        <div class="footer_menu">
            <div class="my_col" v-for="list in footerMenu">
                <h5>{{ list.title.toUpperCase() }}</h5>
                <ul class="list-unstyled">
                    <li v-for="item in list.items">
                        <a href="#">{{ item }}</a>
                    </li>
                </ul>
            </div>
        </div>
        <div class="footer_logo">
        </div>

      </div>
    </div>
    
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
  </footer>
</template>

<style lang="scss" scoped></style>