<script setup>
    import { reactive, ref } from 'vue'
    const items = ref([{ val: 'Himu1' }, { val: 'Himu2' },{ val: 'Himu3' }])


    const myObject = reactive({
        title: 'How to do lists in Vue',
        author: 'Jane Doe',
        publishedAt: '2016-04-10'
    })

</script>

<template>

    <h1>This is List components</h1>
    <li v-bind:key="index" v-for="(item, index) in items">
        {{ index }} - {{ item.val }}
	</li>

    <ul>
        <li :key="value" v-for="value in myObject">
            {{ value }}
        </li>
    </ul>

    <span :key="n" v-for="n in 10">{{ n }}</span>
</template>
