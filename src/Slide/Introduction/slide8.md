---
transition: fade
---

<script setup>
const contents = [
  { text: '<b>Problem:</b> Use <b>multiple</b> <code>print()</code> statements to display your college name and current year on separate lines.' },
  {
    text: '<b>Expected Output:</b><br><code>I study at [Your College Name]</code><br><code>Year: [2024]</code>'
  },
  {
    text: '<b>Note:</b> Write <b>two separate</b> <code>print()</code> statements, one for your college name and one for the year. Replace <code>[Your College Name]</code> with your actual college name and <code>[2024]</code> with the current year. Each string must be wrapped in double quotes <code>" "</code>.'
  }
]
</script>

<Slide
  topic="Getting Started with Python"
  sub-topic="Practice problem"
  :contents="contents"
/>
