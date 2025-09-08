<script>

</script>

<div>
    <p>Skills</p>
    <ul>
        <li>HTML</li>
        <li>CSS</li>
        <li>JavaScript</li>
        <li>Svelte</li>
    </ul>
</div>

<style>
    div {
        display: flex;
        flex-direction: column;
        
        backdrop-filter: blur(4px);
        padding: 2vh 2vw;
        border: 2px solid blue;
        border-radius: 15px;
        width: fit-content;
    }

    p {
        color: var(--color-primary);
        font-size: 1.5rem;
        margin: 0;
    }

    ul {
        list-style-type: square;
        padding-left: 20px;
        margin: 10px 0 0 0;
        color: var(--color-text);
    }

    li {
        margin: 5px 0;
    }
</style>