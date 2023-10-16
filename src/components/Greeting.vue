<template>
<div id="greeting-message">
    <p id="greeting-message-text" style="white-space: pre-line;">{{ greetingMessage }}</p>
</div>
</template>

<script>
export default {
    name: "greeting",
    data() {
        return {
            greetingMessage: 
            `Hello! This is my interactive resume. Thank you for finding it.

            This is an ever-growing project and it's purpose is to put to practice and display my development skills.

            It will be constantly worked on so the state it's in will vary.
            
            Currently I am taking a mobile-first approach, you'll find the best experience to be under 429 x 927
            
            I hope you enjoy!`
        }
    }
}
</script>

<style>
#greeting-message {
    background: repeating-linear-gradient(to bottom, #c0e6ff, #8ea7b8);
    font-size: 24px;
    padding: 5px;
    overflow: none;
}
</style>