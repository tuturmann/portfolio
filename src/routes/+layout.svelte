<header>
    <img src="cat.png" alt="cat icon">
    <p>Applications</p>
</header>

<slot/>

<nav>
    <a href="formation"><img src="formation.png" alt="icône formation"></a>
    <a href="competences"><img src="competences.png" alt="icône compétences"></a>
    <a href="accueil"><img src="accueil.png" alt="icône accueil"></a>
    <a href="projets"><img src="projects.png" alt="icône projets"></a>
    <a href="contact"><img src="phone.png" alt="icône contact"></a>
</nav>

<style>
    nav{
        position:fixed;
        display:flex;
        align-items: center;
        justify-content: center;
        background-color: rgba(255, 255, 255,0.25);
        filter:blur(50%);
        bottom:15px;
        width:50%;
        left:50%;
        transform:translateX(-50%);
        box-sizing: border-box;
        padding:10px 50px;
        border-radius: 23px;
    }

    nav a{
        padding:0px 20px;
    }
    
    @font-face {
        font-family: "EastKind";
        src:
            local("EastKind"),
            url("EastKind.otf") format("opentype");
    }

    header{
        display:flex;
        position:fixed;
        width:100%;
        background-color: #AB5650;
        color:white;
        height:35px;
        align-items: center;
    }

    header>img{
        width:30px;
        height:30px;
        margin-right: 20px
    }

    :global(body){
        margin: 0;
        background-color: #FFF9F0;
    }

    :global(*) {
        font-family: 'Inconsolata', monospace;
    }
</style>