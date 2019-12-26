<script>
    export let ariaLabel = ''
    export let inverted = false
</script>

<button
        aria-label={ariaLabel}
        class:inverted
        on:click
>
    <slot />
</button>

<style>
    button {
        height: 2.25rem;
        min-width: 4rem;
        padding: 0 1rem;
        text-align: center;
        background: none;
        border: 2px solid var(--primary);
        border-radius: .25rem;
        text-transform: uppercase;
    }

    button.inverted {
        color: var(--white);
        border-color: var(--white);
    }

    button:hover,
    button:focus {
        background: var(--primary);
        color: var(--white)
    }

    button.inverted:hover,
    button.inverted:focus {
        background: var(--white);
        color: var(--primary)
    }
</style>
