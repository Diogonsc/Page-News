<template>
    <div class="pure-menu pure-menu-horizontal">
        <div class="container-nav">
            <router-link :to="{ path: '/' }" class="pure-menu-heading pure-menu-link">Home</router-link>
        <ul class="pure-menu-list">
            <li class="pure-menu-item"><router-link :to="{ path: '/new' }" class="pure-menu-link">NEWS</router-link></li>
        </ul>
        <ul class="pure-menu-list">
            <li class="pure-menu-item"><router-link :to="{ path: '/comments' }" class="pure-menu-link">COMMENTS</router-link></li>
        </ul>
        <ul class="pure-menu-list">
            <li class="pure-menu-item"><router-link :to="{ path: '/ask' }" class="pure-menu-link">ASK</router-link></li>
        </ul>
        <ul class="pure-menu-list">
            <li class="pure-menu-item"><router-link :to="{ path: '/jobs' }" class="pure-menu-link">JOBS</router-link></li>
        </ul>
        </div>
    </div>
</template>

<script>
export default {
  name: 'Navbar'
}
</script>

<style scoped>
.logo img {
    width: 120px;
    height: 80px;
}
.pure-menu {
    background-color: #006d77;
}
.pure-menu a {
    color: white;
}

.pure-menu a:hover {
    color:#006d77;
}

  @media (max-width: 760px) {
    .pure-menu .pure-menu-horizontal{
      width:100%;
    }
 }
</style>