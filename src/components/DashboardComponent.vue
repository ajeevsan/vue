<template>
    <div class="container">
        <div class="left">
            <ul>
                <li></li>
                <li></li>
                <li></li>
                <li></li>
            </ul>
        </div>
        <div class="right">
            <div class="rightContainer">
                <div class="graph1"></div>
                <div class="graph2"></div>
            </div>
        </div>
    </div>
</template>

<script>

export default {
    name: 'DashboardComponent',
    props: {
        heading: String,
        options: {
            type: Array
        }
    }
}
</script>
<style>
*,
body {
    margin: 0;
    padding: 0;
    height: 100%;
    width: 100%;
}

.container{
    display: grid;
    grid-template-columns: 2fr 16fr;
    grid-template-rows: 1fr;
}

.left{
    grid-column: 1/2;
    grid-row: 1/2;
    background: red;
    position: relative;
}


.right{
    display: grid;
    grid-template-columns: 1fr;
    grid-template-rows: 1fr;
    grid-column: 2/3;
    grid-row: 1/2;
    background: green;
    position: relative;
}

.rightContainer{
    grid-template-columns: 1fr;
    grid-template-rows: 1fr;
}

</style>