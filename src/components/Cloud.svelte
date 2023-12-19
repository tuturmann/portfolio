<script lang="ts">
    export let name:string;
</script>

<div>
    <img src="right.svg" alt="cloud">
    <span>{name}</span>
</div>

<style>
    div{
        position: absolute;
        display: flex;
        justify-content: center;
        align-items: center;
        top:0;
        right:0;
        height:200px;
        width:250px;

    }

    img{
        height:200px;
        position: absolute;
        top:0;
        right:0;
    }

    span{
        font-family: "TanNimbus";
        font-size: 50px;
        
    }
</style>

