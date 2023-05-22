<script>
export default {
  name: "SiteHeader",
  data() {
    return {
       navItems: [
        {
            name: 'Characters',
            isActive: false 
        },
        {
            name: 'Comics',
            isActive: true 
        },
        {
            name: 'Movies',
            isActive: false 
        },
        {
            name: 'Tv',
            isActive: false 
        },
        {
            name: 'Games',
            isActive: false 
        },
        {
            name: 'Collectibles',
            isActive: false 
        },
        {
            name: 'Videos',
            isActive: false 
        },
        {
            name: 'Fans',
            isActive: false 
        },
        {
            name: 'News',
            isActive: false 
        },
        {
            name: 'Shop',
            isActive: false 
        }
       ] 
    }
    
  }
};
</script>

<template>
  <header>
    <div class="header_container">
      <div class="logo">
        <img src="/img/dc-logo.png" alt="" />
      </div>
      <nav>
        <ul class="list-unstyled d-flex">
          <li class="nav-item" 
          v-for="item in navItems"
          :class="item.isActive === true ? 'active' : ''">
            <a class="nav-link" href="#">
                {{ item.name.toUpperCase() }}
            </a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<style lang="scss" scoped></style>