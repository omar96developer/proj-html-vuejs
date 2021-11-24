<template>
    <li class="mb-3 " >
        <i :class="corse.class"></i>
        {{corse.text}} 
    </li>
    
</template>

<script>
export default {
    name:'ListB',
    props: {
        corse: Array,
    },
    data() {
        return{

        }
    }
}
</script>
<style scoped lang='scss'>
li {
    color: #7abc64;
    
}
</style>