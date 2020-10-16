<template>
    <div class='ui centered card'>
        <div class="content">

        <div class="header">
            {{ todo.title}}
        </div>

        <div class='meta'>
            {{ todo.project }}
        </div>

        <div class="exta content">
            <span class="right floated edit icon">
            <i class="edit icon"></i>
            </span>
        </div>

        <div class='ui bottom attached green basic button' v-show="todo.done">
            Completed
        </div>

        <div class='ui bottom attached red basic button' v-show="!todo.done">
            Completed
        </div>
        </div>
    </div>
</template>

<script type="text/javascript">
    export default {
        props: ['todo'],
    };
</script>