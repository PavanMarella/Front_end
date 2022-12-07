<template>
    <div class="bookbox">


        

        <div v-for="book in books" :key="book.id" >
            <BookItem :book="book"/>
        </div>

    </div>
    


</template>'

<script>

    import BookItem from './BookItem.vue'


    export default{
        name: 'BookBox',
        components: {
            BookItem
        },
        props:{
            
            books: Array,
            nobook:Array
        }
    }

</script>

<style scoped>

.bookbox{

background-color: rgb(238, 190, 131);
padding: 1em;
color: gray;
}

</style>