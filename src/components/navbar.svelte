<nav>
    <div id="name">
        <img src="/coolcat.png" alt="Svelte Logo"  />
        Miami Kittens
    </div>
    
    <ul>
        <li><a href="/">Home</a></li>
        <li><a href="/about">About</a></li>
        <li><a href="/NBA">NBA</a></li>
        <li><a href="/stats">Stats</a></li>
    </ul>
    
</nav>

<style>
    #name img {
        width: 2em;
        height: 2em;
        margin-right: 0.5em;
    }

    #name {
        display: flex;
        align-items: center;
        position: flex-start;
        margin-left: 0em;
        font-size: 1.5em;
    }
    nav {
        font-family: 'Space Font', monospace;
        background-color: #282323;
        padding: 0.5em;
        border: 2px solid #FF69B4;
        box-shadow: 0 0 5px #FF69B4, 0 0 10px #FF69B4, 0 0 20px;
        display: flex;
        justify-content: space-between;
        align-items: center; 
    }
    ul {
        list-style: none;
        padding: 0;
        display: flex;
        justify-content: center;
    }
    li {
        margin-right: 1em;
        display: flex;
        justify-content: center;
        align-items: center;
    }
    a {
        text-decoration: none;
        color: #ffffff;
        justify-content: center;
        align-items: center;
    }
    a:hover {
        text-decoration: underline;
    }
    div {
        color: #ffffff;
        display: flex;
        align-items: center;
        justify-content:flex-start; 
    }
</style>

