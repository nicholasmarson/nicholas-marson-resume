<template>
<div id="greeting-message">
    <p id="greeting-message" style="white-space: pre-line;">{{ greetingMessage }}</p>
</div>
</template>

<script>
export default {
    name: "greeting",
    data() {
        return {
            greetingMessage: 
            `Hello! My name is Nicholas Marson, and this is my interactive resume. Thank you for finding it.

            This is an ever-growing project and it's purpose is to put to practice and display my development skills.

            It will be constantly worked so the state it's in will vary.
            
            Currently I am taking a mobile-first approach, you'll find the best experience to be under 429 x 927`
        }
    }
}
</script>

<style>
#greeting-message {
    font-size: 24px;
    padding: 5px;
}
</style>