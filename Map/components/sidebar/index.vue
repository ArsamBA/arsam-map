<template>
   <v-card>
   <v-layout>
      <v-navigation-drawer
         expand-on-hover
         rail
      >
         <v-list>
         <v-list-item
            :prepend-avatar="information.avatar_url"
            :title="information.title"
            :subtitle="information.email"
         ></v-list-item>
         </v-list>

         <v-divider></v-divider>

         <v-list density="compact" nav>
         <nuxt-link to="/">
            <v-list-item prepend-icon="mdi-home" title="Home page" value="homepage"></v-list-item>
         </nuxt-link>
         <v-list-item prepend-icon="mdi-folder" title="My Files" value="myfiles"></v-list-item>
         <v-list-item prepend-icon="mdi-account-multiple" title="Shared with me" value="shared"></v-list-item>
         <v-list-item prepend-icon="mdi-star" title="Starred" value="starred"></v-list-item>
         </v-list>
      </v-navigation-drawer>

      <v-main style="height: 0px"></v-main>
   </v-layout>
   </v-card>
</template>

<script setup lang="ts">
const information = ref(
   {
      avatar_url : 'https://avatars.githubusercontent.com/u/104560377?v=4',
      title : 'Arsam Bagheramiri',
      email : 'arsam5ba5@gmail.com',
   }
) as any
</script>

<style>

</style>