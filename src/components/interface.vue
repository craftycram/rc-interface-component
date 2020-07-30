<template>
  <b-container>
  <b-row>
    <b-col class="interface embed-responsive embed-responsive-16by9">
      <slot name="videocomponent">
        <img
          class="embed-responsive-item"
          :src="streamUrl"
          alt="Stream kann nicht angezeigt werden">
      </slot>
    </b-col>
  </b-row>
  <b-row>
    <b-col class="interface">
      <slot name="controlcomponent"></slot>
    </b-col>
    <b-col class="interface">
      <slot name="queuecomponent"></slot>
      </b-col>
  </b-row>
</b-container>
</template>

<script>
export default {
  props: {
    streamUrl: String,
  },
};
</script>

<style>
.interface {
  margin: 5px;
  background-color: #eeeeee;
  min-height: 200px;
}

</style>
