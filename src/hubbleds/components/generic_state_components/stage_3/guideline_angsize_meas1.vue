<template>
  <scaffold-alert
    color="info"
    class="mb-4 mx-auto"
    max-width="800"
    elevation="6"
    title-text="Angular Size Measurements"
    @next="state.marker = 'cho_row1'"
    :allow-back="false"
  >
    <template #back-content>
      <div>
        Open menu to return to earlier stages.<br>
        (Open/close menu with <v-icon>mdi-menu</v-icon> above)
      </div>
    </template>
    <div
      class="mb-4"
    >
      <p>
        This is the same sky viewer you used in Stage 1, now with added functionality to measure angular sizes.
      </p>
      <p>
        The green vertical line on the left tells you the <strong>angular size</strong> of the patch of sky being displayed.
      </p>
    </div>
  </scaffold-alert>
</template>

<script>
module.exports = {
 props: ['state']
}
</script>
