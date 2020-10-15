<template>
  <div class="loginForm">

    <!-- Logo -->
    <div class="logo"><img src="/logo.svg" alt="Lyes Hamidi - Web developer designer"></div>
    

    <!-- Title -->
    <h6 class="login__subtitle">Portfolio dashboard</h6>
    <h1 class="login__title">Se connecter</h1>

    <!-- Username -->
    <input type="name" name="username" placeholder="Username">

    <!-- Password -->
    <input type="password" name="password" placeholder="Password">

    <!-- Button send -->
    <button type="submit" class="--disabled">Sign in</button>

    <!-- Follow me -->
    <h6 class="login__subtitle --followme">Follow me</h6>
    <a target="_blank" href="https://www.facebook.com/lyes.ui/" title="Facebook"><img height="16px" src="/svg/facebook.svg" alt="Facebook"></a>
    <a target="_blank" href="https://twitter.com/lyes_ui" title="Twitter"><img height="16px" src="/svg/twitter.svg" alt="Twitter"></a>
    <a target="_blank" href="http://instagram.com/lyes.ui" title="Instagram"><img height="16px" src="/svg/instagram.svg" alt="Instagram"></a>
    <a target="_blank" href="https://www.linkedin.com/in/lyes-hamidi-4b8007174/" title="LinkedIn"><img height="16px" src="/svg/linkedin.svg" alt="LinkedIn"></a>
    <a target="_blank" href="https://dribbble.com/lyes_ui" title="Dribbble"><img height="16px" src="/svg/dribbble.svg" alt="Dribbble"></a>
    <a target="_blank" href="https://www.behance.net/lyes_ui" title="Behance"><img height="16px" src="/svg/behance.svg" alt="Behance"></a>
    <a target="_blank" href="https://github.com/lyesui" title="GitHub"><img height="16px" src="/svg/github.svg" alt="GitHub"></a>
  </div>
</template>

<script>
export default {

}
</script>

<style  lang="scss" scoped>
    .loginForm {
        width: 400px;
        background-color: white;
        box-shadow: 0 10px 50px rgba(0, 0, 0, 0.16);

        padding: 50px;

        border-radius: 10px;

        margin: auto;

        @media (max-width: 400px) {
            width: 90%;

            padding: 50px 32px;
        }

        /* Logo ----------*/
        .logo {
            width: 100%;

            text-align: center;

            margin-bottom: 32px;

            img {
                height: 80px;
            }
        }
        
        /* Title ----------*/
        .login__title {
            color: $black;
            font-size: 32px;
            font-weight: 700;
            line-height: 38px;

            margin-bottom: 11px;
        }

        /* Subtitle ----------*/
        .login__subtitle {
            color: #9D9D9D;
            text-transform: uppercase;
            font-weight: 600;
            font-size: 12px;

            &.--followme {
                color: $black;

                margin-bottom: 6px;
            }
        }

        /* Input ----------*/
        input {
            width: 100%;

            border: 1px solid #E0E0E0;
            border-radius: 4px;

            padding: 14px 18px;
            margin: 7px 0 7px 0;
        }

        input::placeholder {
            color: #E0E0E0;
        }

        /* Button ----------*/
        button {
            width: 100%;
            background-color: $mainColor;

            border-radius: 4px;

            text-align: center;
            color: white;
            font-weight: 600;

            padding: 14px 18px;
            margin: 7px 0 32px 0;

            cursor: pointer;

            &:hover { background-color: #00DDD5; }

            &:focus { background-color: #00B9B3; }

            // Disabled
            &.--disabled {
                background-color: #DDDDDD;

                cursor: auto;

                &:hover {
                    background-color: #CCCCCC;
                }
            }
        }

        /* Social media links ----------*/
        a:not(:last-child) {
            margin-right: 6px;
        }
    }
</style>