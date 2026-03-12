<script>
    let name = "Arno";

    let index = $state("!");

    let game = $state("");

    let size = $state(0);
    function myRoulette() {
        game = "myRoulette";
    }
    function myNothing() {
        game = "Nothing";
    }
    function changeSize() {}
</script>

<head>
    <title>my Epi Casino</title>
</head>

<div>
    <div class="toptopbar"></div>
    <div class="topbar">
        <button>></button>
        <h2>My Epi Casino 🎰</h2>
    </div>
    <div class="layout">
        <div class="sidebar">
            <p>Barre des tâches</p>
            <button><a href="/">Home</a></button>
            <button><a href="/myRoulette">myRoulette</a></button>
            <button>Test2</button>
        </div>
        <div class="content">
            <h1>Bienvenue sur myEpiCasino {index}</h1>
            <h2>Veuillez choisir un jeu : {game}</h2>
            <button onclick={myRoulette} class="button button1"
                ><a href="/myRoulette">myRoulette</a></button
            >
            <button onclick={myNothing} class="button button2">Black</button>
            <h1>TestWelcome</h1>
            <p>does it work?</p>
        </div>
    </div>
</div>

<style>
    @font-face {
        font-family: "MyFont";
        src: url("../fonts/Bileha.otf") format("otf");
        font-weight: normal;
        font-style: normal;
    }

    :global(body) {
        margin: 0;
    }

    /*écritures*/

    h1 {
        color: rgb(255, 255, 255);
        font-family: "MyFont", sans-serif;
        background-color: rgb(41, 41, 41);
        border-radius: 15px;
        padding-left: 15px;
    }

    h2 {
        font-size: 40px;
        font-family: "MyFont", sans-serif;
    }

    /*toptopbar*/

    .toptopbar {
        height: 30px;
        display: flex;
        background-color: rgb(89, 146, 32);
    }

    .topbar {
        height: 70px;
        display: flex;
        background-color: rgb(133, 197, 68);
    }

    .topbar h2 {
        color: white;
        font-family: "MyFont", sans-serif;
        font-size: 30px;
        padding-left: 60px;
        margin-top: 15px;
    }

    .topbar button {
        background-color: #3d3d3d;
        border: grey;
        border-radius: 5px;
        height: 50px;
        margin-top: 10px;
        margin-left: 5px;
        color: white;
    }

    .topbar button:hover {
        background: #222222;
    }

    .layout {
        display: flex;
        height: 100vh;
        background-color: rgb(240, 240, 240);
    }

    /*sidebar*/

    .sidebar {
        border-right: 5px;
        width: 200px;
        background-image: linear-gradient(
            to right,
            rgb(32, 32, 32),
            rgb(34, 34, 34)
        );
        padding: 20px;
        display: flex;
        flex-direction: column;
        border-style: solid;
        border-color: rgb(31, 31, 31);
        gap: 15px;
    }

    .sidebar button {
        padding: 10px;
        border: grey;
        border-radius: 10px;
        border-style: double;
        border-color: #1f1f1f;
        background-color: #111111;
        color: white;
        cursor: pointer;
    }

    .sidebar button:hover {
        background: #010025;
    }

    .sidebar p {
        font-family: "MyFont", sans-serif;
        padding-left: 45px;
        color: white;
    }

    .content {
        flex: 1;
        padding: 30px;
    }

    .content h2 {
        color: white;
    }

    /**button */

    .button {
        border: none;
        color: white;
        padding: 15px 32px;
        text-align: center;
        text-decoration: double;
        display: inline;
        font-size: 16px;
        cursor: grab;
    }

    .button1 {
        border-radius: 10px;
        background-color: #ff0000;
        margin: 0px 50px;
    }

    .button1:hover {
        background-color: #860101;
        padding: 12px 26px;
    }

    .button2 {
        background-color: #202020;
        border-radius: 10px;
        margin: 0px 50px;
    }

    .button2:hover {
        background-color: #000000;
        padding: 12px 26px;
    }
</style>
