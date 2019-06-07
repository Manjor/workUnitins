<template>
    <div id="content">
        <Header />
        <div class="py-3">
            <v-expansion-panel>
                <template v-for="task in tasks">
                    <Task :key="task.id" :id="task.id" :title="task.title" :content="task.content"/>
                </template>
            </v-expansion-panel>
        </div>
    </div>
    
</template>

<script>
import Header from './Header'
import Task from '@/components/task/Task'
export default {
    name: 'Content',
    components:{
        Header, Task
    },
    props:['title'],
    data: function(){
        return{
            tasks: [
                { id: 1, title: 'Titulo 01231311', content: 'Descricao  Da Tarefa'},
                { id: 2, title: 'Titulo 1232321', content: 'Descricao  Da Tarefa'},
                { id: 3, title: 'Titulo 01', content: 'Descricao  Da Tarefa'},
                { id: 4, title: 'Titulo 01', content: 'Descricao  Da Tarefa'},
                { id: 5, title: 'Titulo 01', content: 'Descricao  Da Tarefa'},
                { id: 6, title: 'Titulo 01', content: 'Descricao  Da Tarefa'},
                { id: 7, title: 'Titulo 01', content: 'Descricao  Da Tarefa'},
                { id: 8, title: 'Titulo 01', content: 'Descricao  Da Tarefa'},
                { id: 9, title: 'Titulo 01', content: 'Descricao  Da Tarefa'},
                { id: 10, title: 'Titulo 01', content: 'Descricao  Da Tarefa'},
                { id: 11, title: 'Titulo 01', content: 'Descricao  Da Tarefa'},
                { id: 12, title: 'Titulo 01', content: 'Descricao  Da Tarefa'},
                { id: 13, title: 'Titulo 01', content: 'Descricao  Da Tarefa'},
            ]
        }
    }
}
</script>

<style>

</style>
