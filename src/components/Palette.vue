<template>
    <div class="palette">
        <h2>Current Palette</h2>
        <div v-bind:key="color.id" v-for="color in colors" class="colors-wrap">
            <div class="sample">{{ color.code }}</div>
            {{ color.name }}
            
        </div>
    </div>
</template>

<script>
export default {
   name: "Palette",
   props: ["colors"]
}
</script>

<style scoped>
    .colors-wrap {
        display: flex;
    }
    .sample {
        width: 5em;
        height: 5em;
        border: 1px solid;
        border-radius: 50%;
        display: flex;
        align-items: center;
        justify-content: center;
    }
</style>
