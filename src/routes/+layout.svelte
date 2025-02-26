<slot/>
<script>
    import { onNavigate } from '$app/navigation';

    onNavigate((navigation) => {
        if (!document.startViewTransition) return;

        return new Promise((resolve) => {
            document.startViewTransition(async () => {
                resolve();
                await navigation.complete;
            });
        });
    });
</script>
<style>

    @font-face {
        font-family: "EastKind";
        src: url("/EastKind.otf") format("opentype");
    }
    
    @font-face {
        font-family: "TanNimbus";
        src: url("/TAN-NIMBUS.otf") format("opentype");
    }

    :global(body){
        margin: 0;
        background-color: #FFF9F0;
    }

    :global(*) {
        font-family: 'Inconsolata', monospace;
    }

    :global(img){
        user-select: none;
    }

    :global(html){
        scroll-behavior: smooth;
    }    
    
</style>