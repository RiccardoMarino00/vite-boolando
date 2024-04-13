<script>
export default{
    props: ['type', 'text']

}
</script>




<template>
    <li  :class="`badge--${type}`">{{ text }}</li>
</template>

<style lang="scss">
</style>