<template>
    <div>
         <div class="header">
        <header>
          <div class="logo">
            <img src="~/assets/images/yoga-chakra.jpg" id="yoga-chakra"/>

          </div>
          <h1>Yoga</h1>
        </header>

      </div>
       <div class="nav-bar navbar-expand">
        <nav>
          <ul class="nav-links">
            <li v-for="item in items" v-bind:key="item"><a v-bind:href="item.path">{{item.name}}</a></li>
          </ul>
        </nav>
      </div>
    </div>
</template>

<script>
export default {
    name: 'AppHeader',
    components: {

    },
    data() {
        return {
            items: [{"name":"Home",
      "path":"/"},
      {"name":"About",
      "path":"#/about"},
      {"name":"Yoga",
      "path":"#/yoga" },
      {"name":"Pranayama",
      "path":"#/pranayama"}],
        }
    }
}
</script>