<template>
    <v-card
    class="mx-auto"
    max-width="344"
    outlined
  >
    <v-list-item three-line>
      <v-list-item-content>
        <div class="overline mb-4">
          Математика
        </div>
        <v-list-item-title class="headline mb-1">
            {{task.expiration}}

        </v-list-item-title>
        <v-list-item-subtitle>{{task.description}}</v-list-item-subtitle>
      </v-list-item-content>

      <v-list-item-avatar
        tile
        size="80"
        color="grey"
      ></v-list-item-avatar>
    </v-list-item>

    <v-card-actions>
      <v-btn
        outlined
        rounded
        text @click="accept">
        Button
      </v-btn>
    </v-card-actions>
  </v-card>
</template>

<script>
export default {
    props: ["task"],
    methods:{
      accept(){
        console.log("Accepted task");
      }
    }
}
</script>

<style>

</style>