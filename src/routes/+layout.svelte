<script>

	import { JUPYTERLAB_PATH } from "$env/static/private";

</script>
<svelte:head>
    <script src="https://kit.fontawesome.com/b3bb7373ff.js" crossorigin="anonymous"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="anonymous">
    <link href="https://fonts.googleapis.com/css2?family=Open+Sans&family=Peralta&display=swap" rel="stylesheet">
    <meta name="viewport" content="width=device-width, initial-scale=1">
</svelte:head>

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