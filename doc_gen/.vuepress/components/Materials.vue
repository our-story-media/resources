<template lang="pug">
div(:class="{'pullout':!example}")
    el-card(shadow="never" class="materials")
        div(slot="header")
            i(class="el-icon-tickets")
            strong &nbsp; {{title}}
        slot
</template>

<script>
module.exports = {
    props: ['example','title']
}
</script>

<style>
.materials ul 
{
    margin:0;
}

.materials .el-card__body
{
    padding:1em;
}
</style>