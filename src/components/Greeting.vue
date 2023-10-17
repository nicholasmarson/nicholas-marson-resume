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
            `Hello! Thank you for finding my interactive resume.

            This is an ever-growing project and it's purpose is to display and put to practice my development skills. It will be constantly worked on so the state it's in will vary.
            
            Currently I am taking a mobile-first approach, you'll find the best experience to be under 429 x 927
            
            I hope you enjoy!`
        }
    }
}
</script>

<style>
#greeting-message {
    background: repeating-linear-gradient(to bottom, #edf6fc, #d6eeff);
    font-size: 24px;
    padding: 10px;
    overflow: auto;
}

#greeting-message-text {
    display: flex;
    justify-content: center;
    align-items: center;
    background: repeating-linear-gradient(to bottom, #edf6fc, #d6eeff);
    margin: 0;
    overflow: auto;
}
</style>