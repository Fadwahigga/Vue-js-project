<template>
    <h1>Hello {{ name }} {{ lastName }}</h1>
</template>

<script>
export default {
    props: ['name', 'lastName']
}
</script>

