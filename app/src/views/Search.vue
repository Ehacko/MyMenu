<template>
<div id="recherche" class="vue">
  <div class="content">
    <div class="titre_app">{{$route.name}}</div>
    <input type="text" placeholder="Search restaurant name">
    <ListeRestaurants>
      <CaseRestaurant/>
      <CaseRestaurant/>
    </ListeRestaurants>
    <DropdownMenu/>
  </div>
</div>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component'
import ListeRestaurants from '@/components/ListeRestaurants/ListeRestaurants.vue'
import CaseRestaurant from '@/components/CaseRestaurant/CaseRestaurant.vue'
import DropdownMenu from '@/components/DropdownMenu/DropdownMenu.vue'

@Options({
  components: {
    ListeRestaurants,
    CaseRestaurant,
    DropdownMenu
  }
})
export default class Recherche extends Vue {}
</script>
