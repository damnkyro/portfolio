<div class="container">
    <div>
        <a href="/">
            <img src="/media/2.jpg" alt="pfp" width="50px" class="pfp"/>
        </a>
    </div>

    <div class="flex-container links">
        <a href="/">
            <p>Home</p>
            <img src="/logos/home.svg" alt="home" id="home" width="30px"/>
        </a>
        <a href="/projects">
            <p>Projects</p>
            <img src="/logos/projects.svg" alt="projects" id="projects" width="26px"/>
        </a>
    </div>
</div>

<style>
    .container {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 10px 100px;
        background: #151515;
        box-sizing: border-box;
        
    }

    .pfp {
        border-radius: 100%;
    }
    
    #home, #projects {
        display: none;
    }

    .links {
        display: flex;
        gap: 48px;
    }

    .links a {
        font-size: 16px;
        transition: all ease-in 0.1s;
    }

    .links a:hover {
        color: var(--accent);
    }

    @media screen and (max-width: 768px){
        .container {
            padding: 10px 20px;
        }

        #home, #projects {
            display: flex;
        }

        .links a p {
            display: none;
        }

        .links {
            gap: 26px;
        }
    }
</style>