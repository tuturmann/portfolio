<script lang="ts">
    export let name:string;
</script>

<div>
    <img src="round.png" alt="round shape">
    <span>&gt; {name}</span>
</div>

<style>

    div,img{
        width:350px;
        height:40px;
    }

    div{
        position: relative;
        display:flex;
        justify-content: center;
        align-items: center;
        margin-bottom: 10px;
    }

    img{
        position: absolute;
        top:0;
        left:0;
    }

</style>