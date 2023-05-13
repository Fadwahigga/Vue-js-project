<template>
    <div class="shadow-2xl p-4 w-48 mb-3">
        <!-- <h1 class="shadow-2xl p-4 w-48 mb-3">{{ content }}</h1> -->
        <slot></slot>
    </div>
</template>

<script>
export default {
    props: {
        content: String
    }
}
</script>

