<script>
export default {
    data() {
        return {
            count: 0,
            author: {
                name: 'Jane Doe',
                books: [
                    'Vue 2 - Advanced Guide',
                    'Vue 3 - basic guide',
                ]
            }
        }
    },
    methods: {
        increment() {
            this.count++
        }
    },

    mounted() {
        console.log(this.count)
        this.increment()
    }
}
</script>
<template>
    <h1>Hello Vue</h1>
    <p>This is my app</p>
    <p>Count is {{ count }}</p>
    <button @click="increment">{{ count }}</button>
    <span>{{ author.books.length > 0 ? 'yes' : 'no' }}</span>
</template>