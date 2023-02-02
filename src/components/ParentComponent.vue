<template>
  <div>
    <ul>
      <li v-for="item in items" @click="showContent(item)" :key="item.id" :class="{ active: item === selectedItem }">{{
        item.title
      }}</li>
    </ul>
    <div class="content" v-show="selectedItem === items[0]">
    </div>
    <div class="content" v-show="selectedItem === items[1]">
    </div>
    <div class="content" v-show="selectedItem === items[2]">
    </div>
    <div class="content" v-show="selectedItem === items[3]">
    </div>
  </div>
</template>

<script>

export default {
  name: 'HelloWorld',
  components: {
  },
  data() {
    return {
      items: [        
        { title: 'ENTER CONTENT' },
        {title: 'CUSTOMIZE'},
        {title: 'ADD LOGO', },
        {title: 'DISPLAY' },
      ],
      selectedItem: null
    }
  },
  methods: {
    showContent(item) {
      this.selectedItem = item
    },
  },
}
</script>

<style scoped>
ul {
  margin: 5% 5% 2% 5%;
  display: flex;
  flex-direction: row;
  list-style: none;
  padding: 25px 0;
  border-radius: 25px;
  border: 0.1px solid #099FFF;
  background-color: #18181B;
  box-shadow: 0 4px 8px 0 #00FFFF, 0 6px 20px 0 rgba(0, 0, 0, 0.19);
}

li {
  margin: auto;
  font-size: 20px;
  cursor: pointer;
}

li::after {
  display: block;
  content: '';
  border-bottom: solid 1px #00FFFF;
  padding-bottom: 1%;
  transform: scaleX(0);
  transition: transform 300ms ease-in-out;
}

li:hover::after {
  transform: scaleX(1);
}

.content {
  border-radius: 25px;
  margin: 0 5% 0 5%;
  padding: 25px 0;
  background: #2B3241;
  box-sizing: border-box;
  justify-content: center;
  align-items: center;
}
</style>
