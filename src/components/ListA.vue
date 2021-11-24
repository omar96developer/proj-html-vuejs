<template>
    <li class="mb-3 " >
       <!--  <a :class="links.class ? 'nav-btn' : 'a-1' " :href="links.link">
            {{links.text}}
        </a> -->
        <i class="me-3" :class="contact.class"></i><span>{{contact.text}}</span>
    </li>
    
</template>

<script>
export default {
    name:'ListA',
    props: {
        contact: Array,
    },
    data() {
        return{

        }
    }
}
</script>
<style scoped lang='scss'>
li {
    color: #acb1b7;
}
</style>