<script>
export default {
    props: {
        id: String,
        img: String
    },
}
</script>


<template>
    <div class="image">
        <img :src="img" alt="" >
    </div>
</template>


<style lang="scss">
    
</style>