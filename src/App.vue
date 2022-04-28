<script setup>
// import HelloWorld from './components/HelloWorld.vue'
</script>

<template><body>
<main>
  <link href='https://unpkg.com/boxicons@2.1.2/css/boxicons.min.css' rel='stylesheet'>

            <form>
                <h1>Let's set up your account</h1>
                <p>Already have an account? <a href="/">Sign in</a></p>

                <div class="form-control">
                    <input type="text" placeholder="Your name" required />
                </div>

                <div class="form-control">
                    <input type="email" placeholder="Email address" required />
                </div>

                <div class="form-control">
                    <select name="gender" id="gender">
                        <option>I would describe my user type as</option>
                        <option value="male">Male</option>
                        <option value="female">Female</option>
                        <option value="others">Other</option>
                        <option value="null">Prefer not to say</option>
                    </select>
                </div>

                <div class="form-control">
                    <input type="password" placeholder="Password" required />
                    <i class="bx bx-show"></i>
                    <label for="password">Minimum 8 characters</label>
                </div>

                <button disabled="disabled">Next</button>
                <p>
                    By clicking the "Next" button, you agree to creating a free
                    account, and to <a href="/">Terms of Service</a> and
                    <a href="/">Privacy Policy</a>
                </p>
            </form>
        </main>
        <aside>
            <h3>Dummy Heading</h3>
            <p>
                Lorem ipsum, dolor sit amet consectetur adipisicing elit. Dolor
                totam natus eaque, obcaecati sunt quasi illo excepturi iusto
                dolores, harum ullam cum sit? Harum.
            </p>
        </aside>
        </body>
</template>

<style>
/* @import './assets/base.css'; */
@font-face {
  font-family: "Satoshi-Regular";
  src: local("Satoshi-Regular"),
   url(./fonts/Satoshi-Regular.woff) format("truetype");
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    display: flex;
    min-height: 100vh;
    width: 100vw;
    font-family: "Satoshi", sans-serif;
}

main {
    background: white;
    width: 65%;
    display: flex;
    align-items: center;
    justify-content: center;
}

form {
    max-width: 580px;
    margin-inline: auto;
}

form h1 {
    font-weight: 600;
    margin-bottom: 40px;
}

p {
    color: black;
    margin-bottom: 40px;
}

p a {
    text-decoration: none;
    color: royalblue;
    font-weight: 600;
}

.form-control,
input,
button,
select {
    width: 100%;
}

.form-control {
    margin-bottom: 20px;
}

input,
select,
button {
    padding: 10px;
    color: dimgray;
    font-size: 16px;
    border-radius: 4px;
    border: 1px solid #ccc;
}

label {
    font-size: 12px;
    color: dimgray;
}

button {
    background-color: lightgrey;
    cursor: pointer;
    margin-bottom: 20px;
    font-size: 14px;
}

aside {
    width: 35%;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    gap: 40px;
    background-color: royalblue;
    color: white;
}

aside p {
    max-width: 350px;
    margin-inline: auto;
    color: white;
    line-height: 1.5;
}

.form-control {
    position: relative;
}

.form-control i {
    position: absolute;
    top: 15px;
    right: 5px;
}

@media (min-width: 700px) {
  body {
    font-size: 14px;
  }
}

@media (min-width: 1000px) {
  body {
    font-size: 15px;
  }
}
</style>
