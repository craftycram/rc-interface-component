<template>
  <b-container>
  <b-row>
    <b-col class="grid" style="background-color: yellow; min-height: 720px;">
      Video
      <slot name="videocomponent"></slot>
    </b-col>
  </b-row>
  <b-row>
    <b-col class="grid" style="background-color: cyan; min-height: 200px;">
      controls
      <slot name="controlcomponent"></slot>
    </b-col>
    <b-col class="grid" style="background-color: lightgreen; min-height: 200px;">
      infos / queue
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
