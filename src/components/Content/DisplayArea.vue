<template>
    <div class="container">
                </div>
</template>


<script>

export default {
}
</script>

<style scoped>
*,
*:after,
*:before {
    -webkit-box-sizing: border-box;
    -moz-box-sizing: border-box;
    box-sizing: border-box;
}

@import url('https://fonts.googleapis.com/css2?family=Nunito+Sans:wght@200&display=swap');

:root {
    --font-style: 'Nunito Sans', sans-serif;
}

* {
    box-sizing: border-box;
}

.container {
    position: relative;
    margin-top: 20px;
}

button {
    display: inline-block;
    position: relative;
    background: none;
    border: none;
    color: #fff;
    font-size: 18px;
    cursor: pointer;
    background: #18181B;
}

span {
    display: block;
    padding: 25px 80px;
}

button::before,
button::after {
    content: "";
    width: 0;
    height: 2px;
    position: absolute;
    transition: all 0.2s linear;
    background: #54E6E7;
}

span::before,
span::after {
    content: "";
    width: 2px;
    height: 0;
    position: absolute;
    transition: all 0.2s linear;
    background: #54E6E7;
}

button:hover::before,
button:hover::after {
    width: 100%;
}

button:hover span::before,
button:hover span::after {
    height: 100%;
}

button::after {
    right: 0;
    bottom: 0;
    transition-duration: 0.4s;
}

button span::after {
    right: 0;
    bottom: 0;
    transition-duration: 0.4s;
}

button::before {
    left: 0;
    top: 0;
    transition-duration: 0.4s;
}

button span::before {
    left: 0;
    top: 0;
    transition-duration: 0.4s;
}
</style>
