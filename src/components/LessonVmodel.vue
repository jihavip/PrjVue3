<template>
    <div>
        <p>Nhap vao day: </p><input id="task" type="text" v-model="task"/>
        <button @click="addTask">add</button>
        <button @click="remoteTask">delete</button>
        <br/>
        <p>List vua nhap: </p>
        <ul>
            <li v-for ="todo in todoList" :key="todo">{{todo}}</li>
        </ul>
        <p></p>
        
    </div>
</template>
<script>
export default {
    data() {
        return({
           task:'',
           todoList: []
        })
    },
    methods:{
        addTask(){
            this.todoList.push(this.task)
        },
        remoteTask(){
            this.todoList.pop()
        }
    }
}
</script>
