<template>
  <b-container>
  <b-row>
    <b-col class="grid embed-responsive embed-responsive-16by9" style="background-color: yellow;">
      <slot class="embed-responsive-item" name="videocomponent"></slot>
    </b-col>
  </b-row>
  <b-row>
    <b-col class="grid" style="background-color: cyan; min-height: 200px;">
      <slot name="controlcomponent"></slot>
    </b-col>
    <b-col class="grid" style="background-color: lightgreen; min-height: 200px;">
      <slot name="queuecomponent"></slot>
      </b-col>
  </b-row>
</b-container>
</template>

<script>
export default {

};
</script>

<style>
.grid {
  margin: 5px;
}

</style>
