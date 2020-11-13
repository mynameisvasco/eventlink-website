<script lang="ts">
  export let words: string[] = [""];
  export let delay: number = 1000;
  export let waitToDelete: number = 500;

  let text = "";
  let currentWord = 0;
  let currentLetter = 0;
  let isComplete = false;

  setInterval(() => {
    if (!isComplete) {
      if (currentLetter < words[currentWord].length) {
        text += words[currentWord].charAt(currentLetter);
        currentLetter++;
      } else if (currentLetter == words[currentWord].length) {
        isComplete = true;
      }
    } else {
      if (currentLetter > 0) {
        setTimeout(() => {
          text = text.substring(0, currentLetter - 1);
          currentLetter--;
        }, waitToDelete);
      } else {
        isComplete = false;
        currentLetter = 0;
        if (currentWord < words.length - 1) {
          currentWord++;
        } else {
          currentWord = 0;
        }
      }
    }
  }, delay);
</script>

<div class="inline-flex text-indigo-500 relative flex-row items-center">
  {text}
</div>
