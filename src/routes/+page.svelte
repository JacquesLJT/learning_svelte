<script>
    let username = '';
    let password = '';

    async function handleLogin() {
        // const res = await fetch('http://localhost:3000/api/login', {
        //     method: 'POST',
        //     headers: {
        //         'Content-Type': 'application/json'
        //     },
        //     body: JSON.stringify({ username, password })
        // });

        // if (res.ok) {
        //     const { token } = await res.json();
        //     localStorage.setItem('token', token);
        //     window.location = '/dashboard';
        // } else {
        //     const { error } = await res.json();
        //     alert(error);
        // }
    }
</script>

<div class="page-container">
    <div class="splash-container">
        <h1>Welcome!</h1>
        <p>Please login</p>
    </div>
    <div class="login-container">
        <div class="login-form">
            <h1>Login</h1>
            <input type="text" placeholder="Username" bind:value={username} />
            <input type="password" placeholder="Password" bind:value={password} />
            <button on:click={handleLogin}>Login</button>
        </div>
    </div>
</div>

<style>
    .page-container {
        display: flex;
        flex-direction: row;
        height: 100vh;
        margin: 0;
        padding: 0;
    }
    .splash-container {
        display: flex;
        flex: 3;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        background-color: #faedcd;
    }

    .login-container {
        display: flex;
        flex: 2;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        background-color: #fefae0;
    }
    .login-form {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        background-color: #fff;
        border-radius: 10px;
        box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
        height: 500px;
        width: 500px;
    }
</style>