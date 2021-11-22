<template>
  <div class="note-selectors">
    <NoteSelector v-for="note in notes" v-bind:note="note" v-bind:key="note.id" />
  </div>
</template>

<script>
import NoteSelector from "./NoteSelector.vue";

export default {
  components: {
    NoteSelector,
  },
  data: function () {
    return {
      notes: [
        { id: 1, body: "First note...", timestamp: Date.now() },
        { id: 2, body: "Seconde note...", timestamp: Date.now() },
        { id: 3, body: "Third note...", timestamp: Date.now() },
      ],
    };
  },
};
</script>
