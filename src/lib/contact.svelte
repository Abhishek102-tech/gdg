<script>

</script>

<div>
    <button><a href="https://github.com/Abhishek102-tech">Contact Me</a></button>
</div>

<style>
    div {
        display: flex;
        flex-direction: column;
        margin: 2vh 2vw;
        padding: 2vh 2vw;
        border-radius: 30px;
        width: fit-content;
        border: 0.5px solid var(--COLOR-BORDER);
        box-shadow: 0px 0px 15px 0px var(--COLOR-BORDER);
        background-color: var(--neon-pink);
    }

    button {
        color: var(--color-text);
        border: none;
        padding: 10px 20px;
        font-size: 1rem;
        border-radius: 5px;
        cursor: pointer;
        background: var(--neon-pink);
        position: relative;
        overflow: hidden;
    }

    button:hover {
            animation: glitch 1s infinite;
        }
        button::before, button::after {
            content: '';
            position: absolute;
            top: 0; left: 0; right: 0; bottom: 0;
            z-index: 1;
            pointer-events: none;
            opacity: 0;
        }
        button:hover::before {
            background: repeating-linear-gradient(90deg, #fff 0px, #fff 2px, #000 4px, #000 6px);
            opacity: 0.5;
            animation: glitch-lines 0.3s infinite;
        }
        button:hover::after {
            background: repeating-linear-gradient(0deg, #fff 0px, #fff 2px, #000 4px, #000 6px);
            opacity: 0.5;
            animation: glitch-lines-vert 0.3s infinite;
        }

    @keyframes glitch {
        0% {
            clip-path: inset(0 0 0 0);
            transform: translate(0);
        }
        20% {
            clip-path: inset(10% 0 85% 0);
            transform: translate(-5px, -5px);
        }
        40% {
            clip-path: inset(85% 0 10% 0);
            transform: translate(5px, 5px);
        }
        60% {
            clip-path: inset(10% 0 85% 0);
            transform: translate(-5px, 5px);
        }
        80% {
            clip-path: inset(85% 0 10% 0);
            transform: translate(5px, -5px);
        }
        100% {
            clip-path: inset(0 0 0 0);
            transform: translate(0);
        }
    }

        @keyframes glitch-lines {
            0% { opacity: 0.5; transform: translateY(0); }
            50% { opacity: 1; transform: translateY(-2px); }
            100% { opacity: 0.5; transform: translateY(0); }
        }
        @keyframes glitch-lines-vert {
            0% { opacity: 0.5; transform: translateX(0); }
            50% { opacity: 1; transform: translateX(-2px); }
            100% { opacity: 0.5; transform: translateX(0); }
        }

    button a {
        text-decoration: none;
        color: inherit;
        font-weight: 700;
    }
</style>