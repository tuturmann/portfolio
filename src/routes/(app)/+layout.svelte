<script>
    import { browser } from "$app/environment";
    import { navigating, page } from "$app/stores";
    import { onDestroy, onMount } from "svelte";

    let apptitle = "";

    $: home = $page.route.id === "/(app)/accueil";

    const unsub = navigating.subscribe((n) => {
        if (browser && n) {
            setTimeout(()=>{
                apptitle = document.title;
                console.log(apptitle);
            },100);
        }
    });

    onMount(() => {
        console.log(document.title);
        apptitle = document.title;
    })

    onDestroy(unsub);
</script>

<header>
    <img src="cat.png" alt="cat icon">
    <p>Applications</p>
</header>

{#if !home}
<div class="windowBar">
    <span>{apptitle}</span>
    <a href="accueil"><img src="close.png" alt="closing tab icon"></a>
</div>
{/if}

<slot/>

<nav class:home>
    <a href="presentation"><img src="me.png" alt="icône presentation"></a>
    <a href="formation"><img src="formation.png" alt="icône formation"></a>
    <a href="competences"><img src="competences.png" alt="icône compétences"></a>
    <a href="projets"><img src="projects.png" alt="icône projets"></a>
    <a target="_blank" href="https://manonlclq5.artstation.com"><img src="dessin.png" alt="icône dessins"></a>
    <a href="contact"><img src="phone.png" alt="icône contact"></a>
</nav>

<style>

    .windowBar{
        user-select: none;
        position:fixed;
        top:35px;
        display:flex;
        justify-content: space-between;
        align-items: center;
        color:white;
        background-color: #AB5650;
        width:100%;
        font-size: larger;
        border:2px solid rgb(136, 63, 58);
        z-index: 3;
    }
    .windowBar img{
        margin-right: 15px;
        height:25px;
        width:25px;
    }

    .windowBar span{
        margin-left:15px;
        user-select: none;
    }

    nav{
        user-select: none;
        position:fixed;
        display:flex;
        align-items: center;
        justify-content: center;
        background-color: #AB5650;
        bottom:15px;
        width:50%;
        left:50%;
        transform:translateX(-50%);
        box-sizing: border-box;
        padding:10px 50px;
        border-radius: 23px;
    }

    nav img {
        width:100%;
    }

    .home{
        background-color: rgba(255, 255, 255,0.25);
        filter:blur(50%);
    }

    nav a{
        padding:0px 20px;
    }

    header{
        user-select: none;
        display:flex;
        position:fixed;
        width:100%;
        background-color: #AB5650;
        color:white;
        height:35px;
        align-items: center;
        z-index: 3;
    }

    header>img{
        width:30px;
        height:30px;
        margin-right: 20px
    }

</style>