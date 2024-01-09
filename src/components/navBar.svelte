<script>
   
</script>

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

    <nav class="nav">

        <button class="btn"><a href="/"><i class="fa fa-home"></i></a></button>
        <button class="btn"><a href="/notifications"><i class="fa fa-bell-o"></i></a></button>
        <button class="btn"><a href="/messages"><i class="fa fa-comments"></i></a></button>
        <button class="btn"><a href="/explore"><i class="fa fa-search"></i></button>
        <button class="btn"><a href="/profile"><i class="fa fa-user-circle-o"></i></a></button>
        <button class="btn"><i class="fa fa-cog"></i></button>
    
    </nav>

<style>

    nav {
        position: fixed;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: end;
        top: 0;
        left: 0;
        width: 10vw;
        height: 100vh;
        background-color: var(--dark-purple);
        box-shadow: 1px 0 1px var(--shadow-grey);
    }

    .btn {
        margin-top: 2rem;
        margin-bottom: 2rem;
        margin-right: 1rem;
        width: 3rem;
        height: 3rem;
        border-radius: 0.5rem;
        border-color: white;
        color: var(--dark-purple);
        background-color: white;
        align-items: left;
    }

    .btn:hover {
        cursor: pointer;
    }

    .btn:active, a:active {
        color: var(--medium-purple);
    }

    @media (max-width: 900px) {
        nav {
            width: 90px;
        }
    }

</style>