<template>
  <!-- menu -->
  <div>
    <div class="menu1-box"></div>
    <v-menu
      offset-y
      open-on-hover
      attach=".menu1-box"
      content-class="overflow-visible contain-none"
    >
      <template #activator="{ on, attrs }">
        <v-btn v-bind="attrs" v-on="on">btn</v-btn>
      </template>
      <v-list>
        <!--  -->
        <div class="menu2-box"></div>
        <v-menu
          offset-x
          right
          open-on-hover
          attach=".menu2-box"
          content-class="overflow-visible contain-none"
        >
          <template #activator="{ on, attrs }">
            <v-list-item v-bind="attrs" v-on="on">
              <v-list-item-title>1 ></v-list-item-title>
            </v-list-item>
          </template>
          <v-list>
            <div class="menu3-box"></div>

            <v-list-item>
              <v-list-item-title>1.2</v-list-item-title>
            </v-list-item>
          </v-list>
        </v-menu>
          <!--  -->
          <div class="menu2-box"></div>
        <v-menu
          offset-x
          right
          open-on-hover
          attach=".menu2-box"
          content-class="overflow-visible contain-none"
        >
          <template #activator="{ on, attrs }">
            <v-list-item v-bind="attrs" v-on="on">
              <v-list-item-title>1 ></v-list-item-title>
            </v-list-item>
          </template>
          <v-list>
            <div class="menu3-box"></div>

            <v-list-item>
              <v-list-item-title>1.2</v-list-item-title>
            </v-list-item>
          </v-list>
        </v-menu>

        <!--  -->
        <v-list-item v-bind="attrs" v-on="on">
          <v-list-item-title>2</v-list-item-title>
        </v-list-item>

      </v-list>
    </v-menu>
  </div>
</template>

<script>
export default {

};
</script>

<style lang="scss" scoped>
.contain-none {
  contain: none !important;
}
</style>
