<template>
    <div class="drag-area" ref="dropArea">
        <div class="icon"><i class="fas fa-cloud-upload-alt"></i></div>
    </div>
    <div class="images-container">
    </div>
</template>

<script>
export default {
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@200;300;400;500;600;700&display=swap');

.thumbnail {
    border: 2px solid blue;
}

img {
    margin: 10px 10px 0 20px;
    cursor: pointer;
}

.drag-area {
    border: 10px dashed #1b1b1b;
    /* height: 500px;
    width: 700px; */
    margin: 50px;
    padding: 20px;
    border-radius: 5px;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
}

.drag-area.active {
    border: 10px dashed #B92C2C;
}

.icon {
    font-size: 100px;
}

header {
    font-size: 30px;
    font-weight: 500;
}

span {
    font-size: 25px;
    font-weight: 500;
    margin: 10px 0 15px 0;
}

button {
    padding: 10px 25px;
    font-size: 20px;
    font-weight: 500;
    border: none;
    outline: none;
    background: #18181B;
    color: #00ffff;
    border-radius: 5px;
    cursor: pointer;
}
</style>
