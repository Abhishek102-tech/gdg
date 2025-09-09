<script>
    import calculator from '../assets/calculator.png';
    import Enigma from '../assets/Enigma.png';
    import firstWebsite from '../assets/firstWebsite.png';
    import svgAnimation from '../assets/svgAnimations.png';
</script>

<div>
    <p>Projects</p>
    <ul>
        <li><a href="https://calculator.abhishek.design/"><img src={calculator} alt=""></a></li>
        <li><a href="https://enigma-lyart-two.vercel.app/"><img src={Enigma} alt=""></a></li>
        <li><a href="https://abhishek.design/"><img src={firstWebsite} alt=""></a></li>
        <li><a href="https://newfrontpage.vercel.app/"><img src={svgAnimation} alt=""></a></li>
    </ul>
</div>

<style>
    div {
        width: 63vw;
        display: flex;
        flex-direction: column;
        margin: 0.5vh 0.5vw;
        backdrop-filter: blur(6px);
        padding:0.5vh 0.5vw;
        border-radius: 15px;
        border: 0.5px solid var(--COLOR-BORDER);
        box-shadow: 0px 0px 15px 0px var(--COLOR-BORDER);
    }

    p {
        color: var(--color-text);
        font-size: 2rem;
        margin: 0;
    }

    ul {
        display: flex;
        flex-direction: row;
        gap: 0.5vw;
        color: var(--color-text);
        list-style: none;
        flex-wrap: wrap;
    }

    ul li {
        border: 2px solid var(--color-projects);
        padding: 0.5vw 0.5vh;
        margin: 0.5vh 0.5vw;
        border-radius: 20px;
        box-shadow: 0px 0px 15px 0px var(--neon-pink);
        perspective: 1000px;
    }
    ul li a{
        text-decoration: none;
        margin: 0.5vh 0.5vw;
    }
    ul li a img {
        height: 25vh;
        width: auto;
        margin: 0.5vh 0.5vw;
        transform-style: preserve-3d;
            transition: transform 0.5s cubic-bezier(0.4, 0.2, 0.2, 1);
    }
        ul li a img:hover {
            transform:  rotateY(30deg) rotateX(20deg) rotateZ(10deg) scale(1.05);
            box-shadow: 0 0 15px var(--neon-pink), 0 0 30px var(--neon-pink), 0 0 45px var(--neon-pink);
        }
    @media (max-width: 600px) {
        p {
            font-size: 1rem;
        }
    }
    </style>