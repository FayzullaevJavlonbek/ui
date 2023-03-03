<template>
    <nav>
        <div class="menu-item"><a href="#">Respublika</a></div>
        <Dropdown title="Viloyatlar" :items="region" />
        <Dropdown title="Organizatsiyalar" :items="organisation" />
        <Dropdown title="Kirim-Chiqim" :items="productCRUD" />
        <Dropdown title="Mahsulot-haqida" :items="product" />
   </nav>
</template>   

<script>
import Dropdown from './Dropdown.vue';
export default{
    name: 'navbar',
    components: {
        Dropdown
    },
    data(){
        return {
            organisation: [
                {
                    title: 'Skladlar',
                    link: '#'
                },
                {
                    title: 'Tovarlar',
                    link: '#'
                }
            ],
            region: [
                {
                    title: 'Toshkent',
                    link: '#'
                },
                {
                    title: 'Samarqand',
                    link: '#'
                },
                {
                    title: 'Xiva',
                    link: '#'
                },
                {
                    title: 'Andijon',
                    link: '#'
                },
            ],
            productCRUD:[
                {
                    title: 'Get',
                    link: '#'
                },
                {
                    title: 'Add',
                    link: '#'
                },
                {
                    title: 'Delete',
                    link: '#'
                },
                {
                    title: 'Update',
                    link: '#'
                },
            ],
            product: [
                {
                    title: 'Name',
                    link: '#'
                },
                {
                    title: 'Price',
                    link: '#'
                },
                {
                    title: 'Amount',
                    link: '#'
                }
            ]
        }
    }
}
</script>

    

<style>
nav { 
    display: flex;
    align-items:center;
    justify-content: center;
}
nav .menu-item{
    color: #fff;
    padding: 10px 20px;
    position: relative;
    text-align: center;
    border-bottom: 3px solid transparent;
    display: flex;
    transition: 0.4s;
}
nav .menu-item.active,
nav .menu-item:hover{
    color:aqua;
    background-color: #9f9f9f;
    border-bottom-color: rgb(47, 237, 240);
}
nav .menu-item a {
    color: inherit;
    text-decoration: none;

}
</style>