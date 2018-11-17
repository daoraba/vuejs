<template>
    <div class="card">
        <div class="card-header">Posted {{post.created_at}}</div>
        <div class="card-body">{{post.description}}</div>
        <div class="card-footer">
            <button class="btn btn-default">Edit</button>
            <button class="btn btn-danger">Delete</button>
        </div>
    </div>
</template>

<script>
    export default {
        props: ['post'],
        data () {
            return{
                post: {
                    id: '',
                    description: '',
                    created_at: ''
                }
            }
        },
        mounted() {
            console.log('Component mounted.')
        }
    }
</script>
