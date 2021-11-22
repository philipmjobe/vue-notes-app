<template>
  <div>
    <div class="note-selector" v-for="note in notes" :key="note.id">
      <p class="note-selector-title">{{ note.title }}</p>
      <p class="note-selector-timestamp">{{ note.timestamp }}</p>
    </div>
  </div>
</template>

<script>
export default {
  data: function () {
    return {
      notes: [
        { id: 1, title: "First note...", timestamp: Date.now() },
        { id: 2, title: "Seconde note...", timestamp: Date.now() },
        { id: 3, title: "Third note...", timestamp: Date.now() },
      ],
    };
  },
};
</script>
