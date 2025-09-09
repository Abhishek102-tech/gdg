<script>
    import html from '../assets/html5.svg';
    import css from '../assets/css3.svg';
    import js from '../assets/javascript.svg';
    import svelte from '../assets/svelte.svg';
</script>

<div>
    <p>Skills</p>
    <ul>
        <li><img class="html" src={html} alt="">HTML</li>
        <li><img class="css" src={css} alt="">CSS</li>
        <li><img class="js" src={js} alt="">JavaScript</li>
        <li><img class="svelte" src={svelte} alt="">Svelte</li>
    </ul>
</div>

<style>
    div {
        display: flex;
        flex-direction: column;
        margin: 2vh 2vw;
        backdrop-filter: blur(6px);
        padding: 2vh 2vw;
        border-radius: 15px;
        width: fit-content;
        border: 0.5px solid var(--COLOR-BORDER);
        box-shadow: 0px 0px 15px 0px var(--COLOR-BORDER);
    }

    p {
        color: var(--color-text);
        font-size: 1.5rem;
        margin: 0;
    }

    ul {
        display: flex;
        flex-direction: row;
        list-style-type: square;
        padding-left: 20px;
        margin: 10px 0 0 0;
        color: var(--color-text);
        list-style: none;
    }

    ul img {
  filter: brightness(0) saturate(100%) invert(32%) sepia(100%) saturate(7470%) hue-rotate(303deg) brightness(101%) contrast(101%);
}
    ul li:nth-child(1) img {
        filter: brightness(0) saturate(100%) invert(17%) sepia(100%) saturate(7470%) hue-rotate(270deg) brightness(101%) contrast(101%);
        }
        ul li:nth-child(1):hover img {
            filter: brightness(0) saturate(100%) invert(17%) sepia(100%) saturate(7470%) hue-rotate(270deg) brightness(101%) contrast(101%) drop-shadow(0 0 12px #800080);
    }
    ul li:nth-child(2) img {
        filter: brightness(0) saturate(100%) invert(48%) sepia(100%) saturate(7470%) hue-rotate(293deg) brightness(101%) contrast(101%);
        }
        ul li:nth-child(2):hover img {
            filter: brightness(0) saturate(100%) invert(48%) sepia(100%) saturate(7470%) hue-rotate(293deg) brightness(101%) contrast(101%) drop-shadow(0 0 12px #FF00FF);
    }
    ul li:nth-child(3) img {
        filter: brightness(0) saturate(100%) invert(36%) sepia(100%) saturate(7470%) hue-rotate(245deg) brightness(101%) contrast(101%);
        }
        ul li:nth-child(3):hover img {
            filter: brightness(0) saturate(100%) invert(36%) sepia(100%) saturate(7470%) hue-rotate(245deg) brightness(101%) contrast(101%) drop-shadow(0 0 12px #8A2BE2);
    }
    ul li:nth-child(4) img {
        filter: brightness(0) saturate(100%) invert(32%) sepia(100%) saturate(7470%) hue-rotate(303deg) brightness(101%) contrast(101%);
        }
        ul li:nth-child(4):hover img {
            filter: brightness(0) saturate(100%) invert(32%) sepia(100%) saturate(7470%) hue-rotate(303deg) brightness(101%) contrast(101%) drop-shadow(0 0 12px #FF0099);
    }
    .html{
        height: 11vh;
        vertical-align: middle;
        margin-right: 8px;
        color: var(--color-text);
    }
    .css{
        height: 13vh;
        vertical-align: middle;
        margin-right: 8px;
        color: var(--color-text);
    }
    .js{
        height: 12vh;
        vertical-align: middle;
        margin-right: 8px;
        color: var(--color-text);
    }
    .svelte{
        height: 12vh;
        vertical-align: middle;
        margin-right: 8px;
        color: var(--color-text);
    }
    li {
        border: 3px solid var(--COLOR-BORDER);
        margin: 1vh 1vw;
        font-size: 1.5rem;
        padding: 1.5vh 2vw;
        border-radius: 8px;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        box-shadow: 0 0 6px 4px #800080;
    }
    li:hover {
        box-shadow: 0 0 10px 6px #FF0099, 0 0 10px 7px #800080, 0 0 12px 8px #1E90FF;
        transform: scale(1.05);
        transition: all 0.3s ease-in-out;
        backdrop-filter: blur(8px);
    }
    @media (max-width: 600px) {
        ul {
            flex-wrap: wrap;
            padding-left: 5px;
            gap: 5px;
        }
        li {
            padding: 1vh 1vw;
        }
    }
</style>