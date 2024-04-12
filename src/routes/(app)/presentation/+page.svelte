<script>

    function calculateMyAge() {
        const today = new Date();
        const birthDay = new Date(2004, 11, 5); // month is 0-11, 5th Dec 2004
        let age = today.getFullYear() - birthDay.getFullYear();
        const m = today.getMonth() - birthDay.getMonth();
        if (m < 0 || (m === 0 && today.getDate() < birthDay.getDate())) {
            age--;
        }
        return age;
    }

</script>
<svelte:head>
    <title>Présentation</title>
</svelte:head>

<div class="text">
    <h1>
        Bonjour !
    </h1>
    
    <img class="separator" src="line.png" alt="separator">

    <span>Je suis Manon Leclercq, { calculateMyAge() } ans, étudiante en deuxième année de BUT Informatique à l'IUT A de Lille.</span>
    <span></span>
</div>

<img class="drawing" src="home-portfolio.png" alt="background drawing">


<style>
    span{
        font-size: 25px;
    }
    
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

    span{
        margin-top: 25px;
    }

    h1{
        font-family: "EastKind";
        font-weight: 200;
        color:#AB5650;
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