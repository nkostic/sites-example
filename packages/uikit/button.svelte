<script>
    import { createEventDispatcher } from "svelte"
    const dispatch = createEventDispatcher()
    const handleClick = (event) => {
        dispatch("click", event)
    }
</script>
<button on:click={handleClick}>
    <slot></slot>
</button>
