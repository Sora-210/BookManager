<template>
  <dev>
    <v-btn v-for="btn in btnList" :key="btn.name" @click="$router.push(btn.url)">
      <v-icon>{{btn.icon}}</v-icon>
      <span class="pl-5">{{btn.name}}</span>
    </v-btn>
  </dev>
</template>

<script>
export default {
  name: "Home",
  data: () => ({
    btnList: [
      {
        name:"Home",
        url:"/",
        icon:"fas fa-home"
      },
      // {
      //   name:"検索",
      //   url:"/search",
      //   icon:"fas fa-search"
      // },
      // {
      //   name:"QR",
      //   url:"/qrcodereader",
      //   icon:"fas fa-qrcode"
      // },
      // {
      //   name:"貸出管理",
      //   url:"/admin/rentals",
      //   icon:"fas fa-users-cog"
      // },
      // {
      //   name:"蔵書管理",
      //   url:"/admin/collections",
      //   icon:"fas fa-book"
      // },
      // {
      //   name:"リクエスト管理",
      //   url:"/admin/requests",
      //   icon:"fas fa-envelope-open-text"
      // },
      // {
      //   name:"設定",
      //   url:"/admin/setting",
      //   icon:"fas fa-cog"
      // },
    ]
  })
}
</script>