<template>
    <div class="card">
        <div class="card-header">Test Vuejs + Laravel</div>

        <div class="card-body">
            <!--@if (session('status'))-->
            <!--<div class="alert alert-success" role="alert">-->
                <!--{{ session('status') }}-->
            <!--</div>-->
            <!--@endif-->

            <form action="">
                <div class="form-group">
                    <label for="field">type text:</label>
                    <input type="text" class="form-control" name="field">
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
        mounted() {
            console.log('Component mounted.')
        }
    }
</script>