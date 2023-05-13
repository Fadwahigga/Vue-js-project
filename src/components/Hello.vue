<template>
    <h1>Hello  my name is {{ name }} {{ lastName }} iam {{ age }}</h1>
</template>

<script>
export default {
    // props: ['name', 'lastName']
    props:{
        name:String,
        age:Number
    }
}
</script>

