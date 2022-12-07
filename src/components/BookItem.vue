<template>

    <div :class="book.product_discontinued? 'red': 'green' ">
        <h2> {{book.Watch_series}}</h2>
        <h4> {{book.new_feature[0]}}</h4>
        <h4> {{book.new_feature[1]}}</h4>
        <h4> {{book.new_feature[2]}}</h4>
        <h4> {{book.year_of_release}} </h4>
        <h4> {{book.OS}} </h4>
    </div>

</template>

<script>


export default{
    name: 'BookItem',
    props:{
        book: Array
    }
}


</script>

<style scoped>


h4{
    margin: 2px;
}

div{
    background-color: #09dfee;
    color: black;
    padding: 1em;
}

.red{
background-color: rgb(243, 10, 10) !important;

}
.green{
    background-color: rgb(15, 214, 82);
}


</style>