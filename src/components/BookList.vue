<template>
    <div>
        <h1>{{ title }}</h1>
        <ui>
            <book-item v-for="book in books" :key='book.id' :book='book'></book-item>
        </ui>
    </div>
</template>

<script>
import BookItem from './BookItem';
export default {
    name: 'BookList',
    components: {
        BookItem
    },
    data() {
        return {
            title: 'All Books',
            books: [
                {title: 'Self-Reliance', author: 'Ralph Waldo Emerson'},
                {title: 'American Gods', author: 'Neil Gaiman'},
                {title: 'Amusing Ourselves to Death', author: 'Neil Postman'},
            ]
        }
    }
}
</script>

<style>
    h1, h2 {
        font-weight: normal
    }
    ui {
        list-style-type: none;
        padding: 0;
    }
    li {
        display: block;
        margin: 0 10px;
    }
</style>

