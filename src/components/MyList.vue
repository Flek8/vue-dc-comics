<template>
    
    <ul>
        <li>
            <a href="#">{{element.text}}</a>
        </li>
    </ul>
    
</template>

<script>
export default {
    name: 'MyList',
    props: {
        'element': Object,
        'titolo': String
    }
}
</script>

<style scoped lang="scss">

    li {
        list-style: none;
        margin-left: 10px;
        margin-top: 2px;
    }
    a {
        text-decoration: none;
        color: grey;
    }
</style>