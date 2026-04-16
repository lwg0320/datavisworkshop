---
title: Project Sketches
toc: false
---

<style>
  /* Custom color classes for the grid */
  .text-red { color: #e74c3c; }
  .text-blue { color: #3498db; }
  .text-green { color: #2ecc71; }
  .text-purple { color: #9b59b6; }
  .text-orange { color: #e67e22; }
  .text-teal { color: #1abc9c; }
</style>

<details>
  <summary>Details</summary>
  Something small enough to escape casual notice.
</details>

<div class="grid grid-cols-3">
  <div class="card text-red"><h1>A</h1>1 × 1</div>
  <div class="card text-blue"><h1>A</h1>1 × 1</div>
  <div class="card text-green"><h1>A</h1>1 × 1</div>
  <div class="card grid-colspan-3 text-purple"><h1>B</h1>1 × 3</div>
  <div class="card text-orange"><h1>A</h1>1 × 1</div>
  <div class="card text-teal"><h1>A</h1>1 × 1</div>
  <div class="card text-red"><h1>A</h1>1 × 1</div>
</div>

---

## Dynamic Text Slider

```js
const sampleText = "I want to go to bed.";
const words = sampleText.split(" ");


// Creates a slider from 1 up to the total number of words (6)
const x = view(Inputs.range([1, words.length], {
  step: 1, 
  value: 6, 
  label: "Number of words"
}));


display(words.slice(0, x).join(" "));