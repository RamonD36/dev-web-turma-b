<template>
  <div>
    <div class="section-1">
      <h1>Tarefas</h1>
      <div class="input-group">
        <input class="input-task" type="text" />
        <button class="btn-add-task"><i class="fa-solid fa-plus"></i></button>
      </div>
    </div>
    <ul class="section-2">
      <li v-for="task in tasks" :key="">
        
      </li>
    </ul>
  </div>
</template>

<script>
import { ref } from "vue";
import TaskComponent from "./components/TaskComponent.vue";
const tasks = ref([
  <TaskComponent />
])


export default {
  name: "App",
  components: {
    TaskComponent,
  },
};
</script>

<style>
.section-1 {
  margin: 5% 25% 0 25%;
  display: flex;
  flex-direction: column;
  text-align: start;
  border: solid 2px #2c3e50;
  border-radius: 1em;
  padding: 1em;
}

.section-2 {
    margin: 1em 25%;
}

.section-1 h1 {
  margin: 0;
  margin-bottom: 0.5em;
}

.input-group {
  flex: 1;
  display: flex;
  flex-direction: row;
}

.input-task {
  font-size: 1em;
  padding: 0.5em 0.7em 0.5em 0.7em;
  flex: 1;
  margin-right: 0.5em;
  border: solid 2px #2c3e50;
  border-radius: 50vh;
}
.btn-add-task {
  color: azure;
  background-color: #1ca046;
  width: 40px;
  height: 40px;
  font-size: 1em;
  padding: 0.5em;
  border: none;
  border-radius: 50vh;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
