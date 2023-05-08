<script>

    let email = '';
    let password = '';
    let confirmPass = '';

    function handleAuthenticate() {
        if (!eamil || !password || (register))
    }

</script>
<div class="authContainer" >

    <form action="">

        <h1>Login</h1>
        
        <label>
            <p class={email ? 'above' : "center"}>Email</p>
            <input bind:value={email} type="email" placeholder="Email" />
        </label>
        

        <label>
            <p class={password ? 'above' : "center"}>Password</p>
            <input bind:value={password} type="password" placeholder="Password" />
        </label>
        

        <label>
            <p class={confirmPass ? 'above' : "center"}>Confirm Password</p>
            <input bind:value={confirmPass} type="password" placeholder="Confirm Password" />
        </label>
        <button type="submit">Submit</button>
    </form>
</div>

<style>

    .authContainer {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        flex: 1;
        padding: 24px;
    }
    form {
        display: flex;
        flex-direction: column;
        gap: 8px;
        width: 400px;
        max-width: 100%;
        margin: 0 auto;
    }
    
    form input {
        width: 100%;
        border: none;
        background: transparent;
        color: white;
        padding: 14px;
    }

    form label {
        position: relative;
        border: 2px solid #800080;
        border-radius: 5px;
    }

    h1{
        text-align: center;
    }


    form button {
        background: #800080;
        color:white;
        border: none;
        padding: 10px 0;
        border-radius: 5px;
        cursor: pointer;
        font-size: 1rem;
    }

    form button:hover{
        background: blue;
    }
    
    .above,.center{
        position: absolute;
        transform: translateY(-50%);
        pointer-events: none;
        color: white;
        border-radius: 4px;
        padding: 0 6px;
        font-size: 0.8rem;
    }

    .above{
        top: 0;
        left: 24px;
        background: navy;
        border: 2px solid blue;
        font-size: 0.7rem;
    }
    .error {
        color: coral
    }

    .center {
        top:50%;
        left: 6px;
        border: 1px solid transparent;
        opacity: 0;
    }
</style>
