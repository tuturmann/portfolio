<script lang="ts">

    const skills = [
        {
            name: "java",
            description: "Java est un langage orienté-objet"
        },
        {
            name: "python",
            description: "Python est un langage de programmation que j'ai appris au lycée. Il permet de faire de l'orienté-objet, il possède une large communauté qui apporte de multiples librairies et API. J'ai par exemple utilisé l'API de Discord pour faire un bot."
        },
        {
            name: "sql",
            description: "SQL est un langage qui permet de communiquer avec une base de données."
        },
        {
            name: "linux",
            description: "Linux est un système d'exploitation open-source. J'ai des compétences en BASH, un shell répandu en Linux, j'ai notamment réalisé un <a href=\"projets#projet4\"> morpion </a> dans ce langage."
        },
        {
            name: "html/css",
            description: "HTML/CSS est un langage de style permettant de réaliser des site web en front-end."
        },
        {
            name: "svelte",
            description: "Svelte est un framework liant html, css et javascript. Ce portfolio est codé en Svelte."
        },
        {
            name: "photoshop",
            description: "Photoshop est un logiciel d'édition d'images. Je l'utilise pour dessiner, ainsi que d'autres logiciels concurrents tels que ClipPaint Studio"
        },
        {
            name: "figma",
            description: "Figma est un site web permettant de faire des maquettes de sites web. Je l'ai notamment utilisé pour faire ce portfolio, mais aussi pour tous mes autres projets web."
        }
    ];

    let index = -1;

</script>

<svelte:head>
    <title>Compétences</title>
</svelte:head>

<div class="all">
    <div class="text">
        <h1>Compétences</h1>
        <div class="columns">
            <div class="firstColumn">
                <button on:click={() => index = 0}>&gt; Java</button>
                <button on:click={() => index = 1}>&gt; Python</button>
                <button on:click={() => index = 2}>&gt; SQL</button>
                <button on:click={() => index = 3}>&gt; Linux</button>
            </div>
            <div class="secondColumn">
                <button on:click={() => index = 4}>&gt; HTML/CSS</button>
                <button on:click={() => index = 5}>&gt; Svelte</button>
                <button on:click={() => index = 6}>&gt; Photoshop</button>
                <button on:click={() => index = 7}>&gt; Figma</button>
            </div>
        </div>
    </div>

    <div class="manuel">
        {#if index === -1}
            <p>Cliquez sur une compétence pour voir le texte</p>
        {:else}
            <span>$ man {skills[index].name}</span>
            <p>{@html skills[index].description}</p>
        {/if}
    </div>
</div>
    
<style>
    .manuel :global(a){
        color:white;
    }

    .manuel :global(a:visited){
        color:white;
    }

    .all{
        display:flex;
        width:100%;
        box-sizing: border-box;
        padding:100px 25px 0 25px;
        justify-content: space-between;
    }
    
    .columns{
        display:flex;
        margin:20px;
    }
    
    .columns button{
        text-decoration: underline;
        border:none;
        background: none;
        margin-bottom: 25px;
        font-size: 25px;
    }

    
    .firstColumn,.secondColumn{
        display:flex;
        flex-direction: column;
        font-size: 25px;
        margin-right:50px;
    }

    .manuel{
        background-color: black;
        height:60vh;
        width:50%;
        color: white;
        padding: 10px;
        box-sizing: border-box;
    }

    .text{
        display:flex;
        justify-content: center;
        flex-direction: column;
        width:35%;
    }

    h1{
        font-family: "EastKind";
        font-weight: 200;
        color:#AB5650;
        font-size: 50px;
    }
</style>