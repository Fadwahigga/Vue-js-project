<template>
    <div id="header" class="shadow-2xl p-4 w-48 mb-3">
        <slot name="header"></slot>
    </div>
    <div id="content" class="shadow-2xl p-4 w-48 mb-3 float-right">
        <slot name="content"></slot>
    </div>
    <div id="footer" class="shadow-2xl p-4 w-48 mb-3">
        <slot name="footer"></slot>
    </div>
</template>

<script>
export default {

}
</script>

