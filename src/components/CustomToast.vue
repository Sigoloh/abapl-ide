<template>
    <div class="customToastContainer">
        Brush soaked in <ColorBox :box-color="boxColor"></ColorBox> paint
    </div>
</template>
<style scoped>
.customToastContainer{
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
}
</style>
<script lang="ts">
import ColorBox from "./ColorBox.vue";
export default{
components: {
    ColorBox
},
props:{
    boxColor:{
        type: String,
        required: true
    }
},
setup(props){
    const {boxColor} = props;
    return {
        boxColor,
    }
}
}
</script>