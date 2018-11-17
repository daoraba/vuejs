<template>
    <div class="container">
        <div class="row justify-content-center">
            <div class="col-md-8">
                <form-component></form-component>

                <post-component
                        v-for="post in posts"
                        :key="post.id"
                        :post="post">
                </post-component>
            </div>

        </div>
    </div>
</template>

<script>
    export default {
        data () {
            return{
                posts: [{
                    'id': 1,
                    'description': 'abc',
                    'created_at' : '17/11/2018'
                }]
            }
        },

        mounted() {
            console.log('Component mounted.')
        }
    }
</script>
