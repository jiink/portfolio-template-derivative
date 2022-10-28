<script>
    var t =0;
    const navItems = [
        {title: "About", url: "#About"},
        {title: "Experience", url: "#Experience"},
        {title: "Projects", url: "#Projects"},
        {title: "Museum", url: "#Museum"},
        {title: "Secrets", url: "#Secrets"},
    ]
    setInterval(function () {t++; navItems[2].title = Math.floor(Math.random() * (99 - 11) + 11) + " Projects"}, 1);

    // document.addEventListener('mousemove', (event) => {
	//     navItems[2].title = event.clientX + " Projects";
    // });

    let time = new Date(Date.now());
    const options = {
        weekday: "long",
    };
</script>

<nav>
    <section class="container_nav" id="/">
        {#each navItems as {title, url}}
        <a href={url} class="nav__item"> {title} </a>    
        {/each}
    </section>
    <p class="time">{time.toLocaleDateString(undefined, options)}</p>
</nav>

<style>
    .container_nav{
        display: flex;
        justify-content: center;
        flex-direction: row;
    }

    .nav__item {
        color:rgb(0, 0, 0);
        font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
        font-weight: 600;
        font-size: 2rem;
        margin: 0 2rem;
        transition: 400ms all;
    }

    .nav__item:hover{
        color: purple;
        text-shadow: 0 0 20px rgb(5, 255, 55), 0 0 30px #00ffee, 0 0 40px #4dd0ff, 0 0 50px #4d77ff, 0 0 60px hsl(245, 100%, 65%), 0 0 70px hsl(257, 100%, 65%), 0 0 80px hsl(270, 100%, 65%);
    }

    .time {
    color: #1a1a1a;
    font-weight: 700;
    background-color: #2C91C6;;
    padding: 0.35rem;
    margin: 0 2rem;
    border-radius: 12px;
    }
</style>
