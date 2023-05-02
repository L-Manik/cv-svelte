<div class="parent">
    <div class="sidebar"/>
    <div class="content">
    <slot/>
    </div>
</div>
<style>
    :global(html, body){
        width: 100%;
        height: 100%;
        padding: 0;
        margin: 0;
    }
    .parent {
        width: 100%;
        height: 100%;
        display: flex;
        flex-direction: row;
    }
    .sidebar {
        background-color:rgb(11, 152, 207);
        width: 100px;
        height: 100%;
        margin-right:16px ;
    }
    .content {
        display:flex;
        flex-direction: column;
    }
</style>