<section>
    <div class="container">
        <div>
            <img src="/media/1.jpg" alt="pfp" width="140px" class="pfp"/>
        </div>
    
        <div class="kyro">
            <h2>kyro</h2>
            <p>Full Stack Developer</p>
        </div>
    </div>
</section>

<style>
    .container {
        display: flex;
        align-items: center;
        gap: 32px;
        height: 40vh;
    }

    .kyro {
        display: flex;
        flex-direction: column;
        gap: 18px;
    }

    .kyro h2 {
        font-size: 34px;
        font-weight: 700;
    }
    
    .kyro p {
        color: var(--accent);
        font-size: 16px;
    }

    .pfp {
        border-radius: 100%;        
    }

    @media screen and (max-width: 768px){
        .container {
            flex-direction: column;
            justify-content: center;
            align-items: start;
            margin-bottom: 40px;
        }
    }
</style>