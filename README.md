<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>RIN PANEL</title>

<style>
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    background: #859;
    color: #909;
    font-family: Arial, Helvetica, sans-serif;
    min-height: 100vh;
}

/* ================= LOGIN ================= */

.login-page {
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 34px;
}

.login-card {
    width: 100%;
    max-width: 625px;
    background: #909;
    border: 1px solid #294367;
    border-radius: 27px;
    padding: 48px 50px;
}

.avatar {
    width: 200px;
    height: 200px;
    border-radius: 50%;
    object-fit: cover;
    display: block;
    margin: 0 auto 25px;
}

.login-title {
    text-align: center;
    color: white;
    font-size: 43px;
    font-weight: 700;
    margin-bottom: 12px;
}

.login-subtitle {
    text-align: center;
    color: #8fa5c9;
    font-size: 23px;
    margin-bottom: 54px;
}

label {
    display: block;
    color: #b8c7df;
    font-size: 21px;
    margin-bottom: 12px;
}

input,
select {
    width: 100%;
    height: 75px;
    background: #071122;
    border: 1px solid #304a70;
    border-radius: 15px;
    outline: none;
    color: white;
    font-size: 20px;
    padding: 0 21px;
    margin-bottom: 25px;
}

input:focus,
select:focus {
    border-color: #3474e8;
}

.login-button,
.generate-button {
    width: 100%;
    height: 75px;
    border: 0;
    border-radius: 15px;
    background: #2864df;
    color: white;
    font-size: 21px;
    font-weight: bold;
    cursor: pointer;
}

.login-button:hover,
.generate-button:hover {
    background: #3475ed;
}

/* ================= SAVE PASSWORD ================= */

.remember {
    margin-top: -8px;
    margin-bottom: 25px;
}

.remember-label {
    display: flex;
    align-items: center;
    gap: 10px;

    color: #91a6ca;
    font-size: 17px;

    cursor: pointer;
}

.remember-label input {
    width: 18px;
    height: 18px;
    margin: 0;
    padding: 0;
    accent-color: #2864df;
    cursor: pointer;
}

/* ================= REGISTER ================= */

.register {
    text-align: center;
    margin-top: 34px;
    color: #91a6ca;
    font-size: 20px;
}

.register a {
    color: #4b8df5;
    text-decoration: none;
}

/* ================= DASHBOARD ================= */

.dashboard {
    display: none;
    width: 100%;
    max-width: 700px;
    margin: 0 auto;
    padding: 35px;
}

.alert {
    background: #073524;
    border: 1px solid #138457;
    color: #d5eee4;
    border-radius: 22px;
    padding: 25px 34px;
    font-size: 25px;
    margin-bottom: 30px;
}

.card {
    background: #0c1729;
    border: 1px solid #294367;
    border-radius: 23px;
    padding: 34px;
    margin-bottom: 34px;
}

.card h2 {
    color: white;
    font-size: 40px;
    margin-bottom: 35px;
}

.card label {
    font-size: 26px;
    color: #aebed8;
}

.card input,
.card select {
    height: 75px;
    font-size: 20px;
}

/* ================= LICENSES ================= */

.license {
    padding: 0 0 25px;
    margin-bottom: 27px;
    border-bottom: 1px solid #263c5b;
}

.license-key {
    color: #75a9ff;
    font-size: 25px;
    font-weight: bold;
    margin-bottom: 13px;
    word-break: break-all;
}

.license-info {
    color: #91a6c8;
    font-size: 22px;
    line-height: 1.8;
}

.buttons {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 13px;
    margin-top: 12px;
}

.action {
    height: 70px;
    border: 0;
    border-radius: 15px;
    color: white;
    font-size: 20px;
    font-weight: bold;
    cursor: pointer;
}

.active {
    background: #128a43;
}

.inactive {
    background: #aa7000;
}

.ban {
    background: #7022b2;
}

.delete {
    background: #ad2638;
}

/* ================= MOBILE ================= */

@media (max-width: 600px) {

    body {
        width: 100%;
        overflow-x: hidden;
    }

    .login-page {
        min-height: 100vh;
        padding: 16px;
        align-items: center;
    }

    .login-card {
        width: 100%;
        max-width: 100%;
        padding: 28px 22px;
        border-radius: 20px;
    }

    .avatar {
        width: 120px;
        height: 120px;
        margin-bottom: 18px;
    }

    .login-title {
        font-size: 30px;
        margin-bottom: 8px;
    }

    .login-subtitle {
        font-size: 16px;
        margin-bottom: 30px;
    }

    label {
        font-size: 16px;
        margin-bottom: 8px;
    }

    input,
    select {
        width: 100%;
        height: 54px;
        font-size: 16px;
        padding: 0 14px;
        margin-bottom: 18px;
        border-radius: 11px;
    }

    .remember-label {
        font-size: 14px;
    }

    .remember-label input {
        width: 17px;
        height: 17px;
    }

    .login-button,
    .generate-button {
        height: 54px;
        font-size: 16px;
        border-radius: 11px;
    }

    .register {
        font-size: 15px;
        margin-top: 22px;
    }


    /* DASHBOARD */

    .dashboard {
        width: 100%;
        max-width: 100%;
        padding: 16px;
    }

    .alert {
        padding: 16px 18px;
        font-size: 16px;
        border-radius: 14px;
        margin-bottom: 18px;
    }

    .card {
        padding: 22px 18px;
        border-radius: 18px;
        margin-bottom: 20px;
    }

    .card h2 {
        font-size: 27px;
        margin-bottom: 24px;
    }

    .card label {
        font-size: 16px;
    }

    .card input,
    .card select {
        height: 54px;
        font-size: 16px;
    }

    .license-key {
        font-size: 18px;
    }

    .license-info {
        font-size: 15px;
        line-height: 1.7;
    }

    .buttons {
        gap: 8px;
    }

    .action {
        height: 48px;
        font-size: 14px;
        border-radius: 10px;
    }
}
    }
}
</style>
</head>

<body>

<!-- ================= LOGIN PAGE ================= -->

<div class="login-page" id="loginPage">

    <div class="login-card">

        <img src="avatar.jpg" class="avatar" alt="Avatar">

        <h1 class="login-title">
            RIN PANEL
        </h1>

        <p class="login-subtitle">
            Secure License Management
        </p>

        <label for="username">
            Username or Email
        </label>

        <input
            type="text"
            id="username"
            autocomplete="username"
        >

        <label for="password">
            Password
        </label>

        <input
            type="password"
            id="password"
            autocomplete="current-password"
        >

        <!-- SAVE PASSWORD -->

        <div class="remember">
            <label class="remember-label">
                <input
                    type="checkbox"
                    id="remember"
                >
                <span>Save password</span>
            </label>
        </div>

        <button
            class="login-button"
            onclick="login()"
        >
            LOGIN
        </button>

        <p class="register">
            Don't have an account?
            <a href="#">Register</a>
        </p>

    </div>

</div>


<!-- ================= DASHBOARD ================= -->

<div class="dashboard" id="dashboard">

    <div class="alert">
        License activated.
    </div>

    <!-- CREATE LICENSE -->

    <div class="card">

        <h2>
            Create License
        </h2>

        <label for="game">
            Game
        </label>

        <select id="game">
            <option>CODMGR</option>
        </select>

        <label for="devices">
            Max Devices
        </label>

        <input
            type="number"
            id="devices"
            value="1"
            min="1"
        >

        <label for="duration">
            Duration Days
        </label>

        <input
            type="number"
            id="duration"
            value="1"
            min="1"
        >

        <label for="bulk">
            Bulk Keys
        </label>

        <input
            type="number"
            id="bulk"
            value="1"
            min="1"
        >

        <label for="prefix">
            Custom Prefix
        </label>

        <input
            type="text"
            id="prefix"
            value="RIN"
        >

        <button
            class="generate-button"
            onclick="generateLicense()"
        >
            GENERATE LICENSE
        </button>

    </div>


    <!-- GENERATED LICENSES -->

    <div class="card">

        <h2>
            Generated Licenses
        </h2>

        <div id="licenses"></div>

    </div>

</div>


<script>

/* ================= LOGIN ================= */

function login() {

    const username =
        document.getElementById("username").value.trim();

    const password =
        document.getElementById("password").value;

    const remember =
        document.getElementById("remember").checked;


    /*
        DEMO LOGIN
        Username: admin
        Password: admin123
    */

    if (
        username === "admin" &&
        password === "admin123"
    ) {

        if (remember) {

            localStorage.setItem(
                "rin_username",
                username
            );

            localStorage.setItem(
                "rin_password",
                password
            );

            localStorage.setItem(
                "rin_remember",
                "true"
            );

        } else {

            localStorage.removeItem(
                "rin_username"
            );

            localStorage.removeItem(
                "rin_password"
            );

            localStorage.removeItem(
                "rin_remember"
            );
        }


        document.getElementById("loginPage")
            .style.display = "none";

        document.getElementById("dashboard")
            .style.display = "block";

    } else {

        alert("Invalid username or password.");

    }
}


/* ================= LOAD SAVED LOGIN ================= */

window.addEventListener(
    "DOMContentLoaded",
    function () {

        const savedUsername =
            localStorage.getItem("rin_username");

        const savedPassword =
            localStorage.getItem("rin_password");

        const savedRemember =
            localStorage.getItem("rin_remember");


        if (
            savedUsername &&
            savedPassword &&
            savedRemember === "true"
        ) {

            document.getElementById("username").value =
                savedUsername;

            document.getElementById("password").value =
                savedPassword;

            document.getElementById("remember").checked =
                true;
        }

    }
);


/* ================= RANDOM CODE ================= */

function randomCode(length = 10) {

    const chars =
        "ABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789";

    let result = "";

    for (let i = 0; i < length; i++) {

        result += chars.charAt(
            Math.floor(
                Math.random() * chars.length
            )
        );
    }

    return result;
}


/* ================= GENERATE LICENSE ================= */

function generateLicense() {

    const game =
        document.getElementById("game").value;

    const devices =
        document.getElementById("devices").value;

    const duration =
        document.getElementById("duration").value;

    const bulk =
        parseInt(
            document.getElementById("bulk").value
        );

    const prefix =
        document.getElementById("prefix").value.trim();

    const container =
        document.getElementById("licenses");


    if (!bulk || bulk < 1) {

        alert("Bulk Keys must be at least 1.");

        return;
    }


    for (let i = 0; i < bulk; i++) {

        const key =
            "1x" +
            prefix.toUpperCase() +
            "-" +
            randomCode(10);

        const license =
            document.createElement("div");

        license.className = "license";


        license.innerHTML = `

            <div class="license-key">
                ${key}
            </div>

            <div class="license-info">

                ${game} /
                ${duration} Days /
                ${devices} Devices

                <br>

                Activated: Not yet

                <br>

                Expires: Starts on first login

                <br>

                Status: ACTIVE

            </div>

            <div class="buttons">

                <button
                    class="action active"
                    onclick="changeStatus(this, 'ACTIVE')"
                >
                    ACTIVE
                </button>

                <button
                    class="action inactive"
                    onclick="changeStatus(this, 'INACTIVE')"
                >
                    INACTIVE
                </button>

                <button
                    class="action ban"
                    onclick="changeStatus(this, 'BANNED')"
                >
                    BAN
                </button>

                <button
                    class="action delete"
                    onclick="deleteLicense(this)"
                >
                    DELETE
                </button>

            </div>
        `;

        container.prepend(license);
    }
}


/* ================= STATUS ================= */

function changeStatus(button, status) {

    const license =
        button.closest(".license");

    const info =
        license.querySelector(".license-info");

    const lines =
        info.innerHTML.split("<br>");

    lines[3] =
        "Status: " + status;

    info.innerHTML =
        lines.join("<br>");
}


/* ================= DELETE ================= */

function deleteLicense(button) {

    const license =
        button.closest(".license");

    license.remove();
}

</script>

</body>
</html>
