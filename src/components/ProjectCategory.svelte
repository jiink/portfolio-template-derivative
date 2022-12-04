<script>
    export let categoryName;
    export let categoryIcon;
</script>


<header style="display: flex; align-items: center;">
    <img src="{categoryIcon}" alt="icon" width="32" height="32" style="image-rendering: pixelated;"/>
    <span style="margin-left: 30px;">{categoryName}</span>
</header>


<style>

    span {
        line-height: 2;
        font-size: 30px;
        color: white;
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
