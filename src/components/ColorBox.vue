<template>
    <div class='colorBoxContainer' :style="{background: boxColor}">
    </div>
</template>
<style scoped>
.colorBoxContainer{
    width: 15px;
    height: 15px;
    margin-left: 5px;
    margin-right: 5px;
}
</style>
<script lang="ts">
export default{
    props: {
        boxColor: {
            type: String,
            required: true
        }
    },    
    setup(props){
        const {boxColor} = props;
        return {
            boxColor,
        };
    }
}
</script>