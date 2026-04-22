<template>
    <div @click="markCompleted" class="task" :class="{'task-complete' : isComplete}">
        <p>{{ taskDescripton }}</p>
        <button><i class="fa-solid fa-xmark"></i></button>
    </div>
</template>

<script>
export default {
    name: "TaskComponent",
    data() {
        return {
            taskDescripton: "Descrição da tarefa",
            isComplete: false,
        };
    },

    methods: {
        markCompleted() {
            this.isComplete = !this.isComplete;
}

    },
};


</script>

<style>
:scope .task {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    border: solid 2px #2c3e50;
    border-radius: 1em;
    padding: 1em;
}

.task-complete {
    text-decoration: line-through;
    opacity: 50%;
}

.task p {
    margin: 0;
}

.task button {
    color: azure;
    background-color: #cc3a3a;
    margin: 0;
    margin-left: 0.5em;
    width: 2em;
    height: 2em;
    border: none;
    border-radius: 5vh;
}
</style>