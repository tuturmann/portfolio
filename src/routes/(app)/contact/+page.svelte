
<svelte:head>
    <title>Contact</title>
</svelte:head>

<div class="text">
    <h1>
        Contact
    </h1>
    
    <img class="separator" src="line.png" alt="separator">
    <div class="imagentext">
        <img src="envelope.png" alt="envelope logo">
        <a target="_blank" href="mailto:manon.leclercq7.etu@univ-lille.fr">manon.leclercq7.etu@univ-lille.fr</a>
    </div>
    <div class="imagentext">
        <img src="github.png" alt="github logo">
        <a target="_blank" href="https://github.com/tuturmann">tuturmann</a>
    </div>
    <div class="imagentext">
        <img src="linkedin.png" alt="linkedin logo">
        <a target="_blank" href="https://www.linkedin.com/in/manon-l-789108264/">Manon Leclercq</a>
    </div>
    <div class="imagentext">
        <img src="gitlab.png" alt="gitlab logo">
        <a target="_blank" href="https://gitlab.univ-lille.fr/manon.leclercq7.etu">@manon.leclercq7.etu</a>
    </div>
    <div class="imagentext">
        <img src="gitlab.png" alt="CV logo">
        <a target="_blank" href="/cv.pdf">Mon CV</a>
    </div>

</div>

<img class="drawing" src="home-portfolio.png" alt="background drawing">


<style>
    .text{
        margin: 15px;
        display:flex;
        justify-content: center;
        align-items: start;
        flex-direction: column;
        position:fixed;
        top: 60px;
        width:35%;
        
    }

    .imagentext{
        display: flex;
        align-items: center;
        margin-top:40px;
        margin-left: 20px;
    }

    .imagentext img{
        width:25px;
        height:25px;
    }

    .imagentext a{
        margin-left: 50px;
        color:black;
        text-decoration: underline;
        
    }


    h1{
        font-family: "EastKind";
        color:#AB5650;
        font-weight: 200;
        font-size: 50px;
    }

    .drawing{
        float:right;
        
        height:100vh;
        z-index: -1;
    }
    .separator{
        width:75%;
    }

</style>