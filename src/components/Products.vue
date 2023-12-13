<template>
    <div>
        <div class="container">
        <h2>Child Component</h2>
        <p> {{ greeting }}</p>
    </div>

    </div>
</template>

<script>
    export default {
        name: 'ProductComp',
        props: ['greeting']
    }
</script>

<style scoped>
.container{
    background-color: rgba(68, 68, 208, 0.44);
}
    
</style>