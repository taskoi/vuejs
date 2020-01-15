<template>
    <div>
        <div class="title">
            <slot name="title"></slot>
            <span>
                <slot style="color: #ccc" name="subtitle">The subtitle</slot>
            </span>
        </div>
        <hr>
        <div>
            <slot></slot>
        </div>
    </div>
</template>

<script>
    export default {}
</script>

<style scoped>
    div {
        border: 1px solid black;
        box-shadow: 1px 1px 2px black;
        padding: 30px;
        margin: auto;
        text-align: center;
    }

    h2 {
        color: red;
    }

    .title {
    }
</style>