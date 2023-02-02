<template>
  <div class="gradient-input">
    <div>
    
    </div>
    
    <div>
    
    </div>
  </div>
  <div class="gradient-input">
    <div>
    
    </div>
    
    <div>
    
    </div>
  </div>
</template>

<script>
export default {
  name: "ContentTwo",
}
</script>

<style scoped>
label {
  /* display: flex; */
  align-items: center;
  margin-bottom: 10px;
}

input[type="number"] {
  width: 80px;
  padding: 5px;
  border-radius: 5px;
  border: 1px solid #ccc;
}

span {
  margin-left: 10px;
}

input[type="text"] {
  width: 50%;
  font-size: 16px;
  color: #00FFFF;
  margin-bottom: 30px;
  margin-left: 10px;
  text-align: center;
  border: none;
  border-bottom: 2px solid #00FFFF;
  outline: none;
  background: transparent;
}

input[type="number"] {
  width: 50%;
  font-size: 16px;
  color: #00FFFF;
  margin-bottom: 30px;
  margin-left: 10px;
  text-align: center;
  border: none;
  border-bottom: 2px solid #00FFFF;
  outline: none;
  background: transparent;
}

input[type="color"] {
  -webkit-appearance: none;
  border: none;
  background: transparent;
}

input[type="color"]::-webkit-color-swatch {
  border: none;
}
</style>
