<template>
    <div>
        <div class="footer">
            <ul>
                <li>lorem</li>
                <li>lorem</li>
                <li>lorem</li>
            </ul>
        </div>
    </div>
</template>


<script>
export default {
    name:'foot'
    
}
</script>

<style  scoped>
.footer{
    width: 100%;
    color:white;
    background-color: black;
    font-family: sans-serif;
    height: 80px;
    direction: flex;
    align-items: center;
}

ul{
    display: flex;
    justify-content: space-around;
    align-items: center;
    list-style: none;
    
}

ul li{
margin-top: 30px;
}
</style>