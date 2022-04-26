<template>
    <div>
        <input id="task" type="text" v-model="task"/>
        <p>Da nhap vao: {{task}}</p>
    </div>
</template>
<script>
export default {
    data() {
        return({
            task: ''
        })
    },
}
</script>
