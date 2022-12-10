<script>
    export let categoryName;
    export let categoryIcon;
    
</script>


<header style="display: flex; align-items: center; justify-content: space-between;">
    <img src="{categoryIcon}" alt="icon" width="38" height="38" style="image-rendering: pixelated; margin-right: 30px;"/>
    <span style="flex-grow: 1;">{categoryName}</span>
    <img src="\assets\expandicon.png" alt="icon" width="38" height="38" style="image-rendering: pixelated; margin-right: 86px"/>
</header>


<style>
    @font-face {
        font-family: 'Garamond';
        src: url('../assets/GARABD.TTF') format('truetype');
    }

    span {
        font-family: 'Garamond';
        line-height: 1.4;
        font-size: 50px;
        color: rgb(255, 255, 255);
    }

    header {
        top: 0px;
        left: 0;
        right: 0;
        background-color: #342C39;
        text-align: left;
        padding-left: 30px;
        padding-top: 0px;
        margin-top: 20px;
        padding-bottom: 0px;
    }
</style>
