<template>
    <ul>
        <li v-for="(element, index) in msg" :key="index">
            <a href="#">{{element.text}}</a>
        </li>
    </ul>
</template>

<script>
export default {
    name: 'MyList',
    props: {
        msg: String
    }
}
</script>

<style scoped lang="scss">

</style>