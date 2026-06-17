---
transition: fade
---

<script setup>
const contents = [
  { text: '<b>#</b> — Lines starting with <strong>#</strong> are comments. Python skips them.' },
  {
    text: '<b>print()</b> — Displays whatever is inside the brackets.'
  },
  {
    text: '<b> "..." </b> — Double quotes wrap a string (text) value.'
  }
]
</script>

<Slide
  topic="Getting Started with Python"
  sub-topic="First Program in Python🎉"
  :contents="contents"
/>
