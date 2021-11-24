<template>
    <li >
        <a :class="links.class ? 'nav-btn' : 'a-1' " :href="links.link">
            {{links.text}}
        </a>
    </li>
</template>

<script>
export default {
    name:'Navbar',
    props: {
        links: Array,
    },
    data() {
        return{

        }
    }
}
</script>
<style scoped lang='scss'>
.a-1{
    text-decoration: none;
    color: white;
    padding-bottom: 10px;
    &:hover{
        color: #7abc64;
        border-bottom: 4px solid #7abc64;
    }
}

 .nav-btn{
    background-color: #7abc64;
    color: white;
    border-radius: 15px;
    text-decoration: none;
    padding: 5px 15px;
    &:hover {
        color: #7799ad;
        border: 3px solid #7799ad;
        border-radius: 20px;           
        background-color: white;
    }
    } 
</style>