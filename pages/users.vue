<template>
  <div class="tile is-ancestor">
    <div class="tile is-parent">
      <div class="tile is-child box">
        <p class="title">Users</p>
        <p>This page is CLUD Sample.</p>
        <br />
        <user-edit />
      </div>
    </div>
  </div>
</template>

<script>
import UserEdit from "~/components/UserEdit.vue";

export default {
  components: {
    UserEdit
  }
};
</script>

