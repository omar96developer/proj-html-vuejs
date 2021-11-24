<template>
    <li >
        <a class="d-flex" :class="links.class ? 'nav-btn' : 'a-1' " :href="links.link" >
            {{links.text}}
            <span class="badge" :class="(links.text == 'COURSES') ? 'active' : ''">{{newt}}</span>
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
            newt: 'New'
        }
    }
}
</script>
<style scoped lang='scss'>
span{
    display: none;
    &.active {
        display: flex;
        background-color: #7abc64;
        margin-left: 5px;
        padding: 1px 9px;
        align-items: center;
        
    }
}
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
    border-radius: 20px;
    text-decoration: none;
    padding: 5px 15px;
    border: 3px solid rgba(0, 0, 0, 0.5);

    &:hover {
        background-color: white;
        border: 3px solid #7abc64;
        color: #7abc64;
        border-radius: 20px;
    }
    } 
</style>