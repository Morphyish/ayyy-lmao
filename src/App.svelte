<script>
    import Button from './components/Button.svelte'
    import Game from './Game.svelte'

    let started = false
</script>

<Button
        ariaLabel="Start"
        on:click={() => started  = true}
>
    Start
</Button>

<Game {started} />
