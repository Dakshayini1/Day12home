 ## Real-time Character Counter

This is a simple real-time character counter that counts the number of characters in a textarea and displays the total number of characters and the number of remaining characters.
# Hosted Link
https://Dakshayini1.github.io/Day12home/
### Step-by-Step Explanation

#### HTML

The HTML code creates a simple webpage with a textarea and two paragraphs to display the total number of characters and the number of remaining characters.



#### CSS

The CSS code styles the textarea and the counter container.



#### JavaScript
```
const textareaEl = document.getElementById("textarea");
const totalCounterEl = document.getElementById("total-counter");
const remainingCounterEl = document.getElementById("remaining-counter");

textareaEl.addEventListener("keyup", () => {
  updateCounter();
});

updateCounter()

function updateCounter() {
  totalCounterEl.innerText = textareaEl.value.length;
  remainingCounterEl.innerText =
    textareaEl.getAttribute("maxLength") - textareaEl.value.length;
}
```
