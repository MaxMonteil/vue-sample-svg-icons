<template>
  <section>
    <h2>Regular Icons</h2>
    <p class="info">All found on <a href="https://icomoon.io/" target="_blank">Icomoon</a>, using the Vicons set</p>
    <p>
      <!--you can pass in a smaller width and height using the size prop-->
      <icon-base size="12" icon-name="write" />
      <!--or you can use the default, which is 18-->
      <icon-base icon-name="write" />
      <!--or make it a little bigger too :) -->
      <icon-base size="30" icon-name="write" />
      <br>
      You can make inline icons of any size by passing props.
    </p>
    <p style="color:red">
      <!--you can change the color of the text, and the icons will automatically change color as well-->
      <icon-base icon-name="moon" />
      These red inline icons are automatically styled according to the text color.
    </p>
    <p>
      <!--because the base is consistent, you can use multiple icons on the same line and they're all in order-->
      <icon-base icon-name="moon" />
      <icon-base icon-name="write" />
      <icon-base icon-name="image" />
      <icon-base icon-name="garbage" />
      <icon-base icon-name="calendar" />
      <icon-base icon-name="envelope" />
      <br>
      <icon-base />
      You can use whatever icon you want and keep the base consistent with slots
    </p>
  </section>
</template>

<script>
import IconBase from './IconBase.vue'

export default {
  components: {
    IconBase
  }
}
</script>
