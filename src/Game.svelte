<script>
    export let started = false
</script>

<div id="game" class:started></div>

<style>
    #game {
        position: fixed;
        top: 50%;
        left: 50%;
        height: 0;
        width: 0;
        overflow: hidden;
        background: var(--primary);
        transition: none;
    }

    #game.started {
        top: 0;
        left: 0;
        width: 100vw;
        height: 100vh;
        transition: top 225ms ease,
        left 225ms ease,
        height 225ms ease,
        width 225ms ease;
    }
</style>
