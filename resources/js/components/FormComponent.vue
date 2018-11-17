<template>
    <div class="card">
        <div class="card-header">Test Vuejs + Laravel</div>

        <div class="card-body">

            <form action="" v-on:submit.prevent="newPost()">
                <div class="form-group">
                    <label for="field">type text:</label>
                    <input type="text" class="form-control" name="field"
                    v-model="description">
                </div>
                <button type="submit" class="btn btn-primary">
                    Send Post
                </button>
            </form>

        </div>
    </div>
</template>

<script>
    export default {
        data(){
            return {
                description:''
            }
        },
        mounted() {
            console.log('Component mounted.')
        },
        methods: {
            newPost() {
                alert(this.description);
            }
        }
    }
</script>