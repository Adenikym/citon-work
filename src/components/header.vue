<template>
    <div class="header">
        
        <h1 class="mini">Mini Blog</h1>
        
    </div>
</template>

<script>
export default {
    name:"blogheader"
}
</script>

<style  scoped>
*{
    margin:0;
    padding: 0;
    box-sizing: border-box;
}
.header{
    height:150px;
    color:#e75480;
    background-color: #212121;
    display:flex;
    justify-content: center;
    align-items: center;
}

.mini{
    font-size: 60px;
}
</style>