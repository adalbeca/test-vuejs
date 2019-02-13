<template>
    <div class="container ">
        <div class="row p-2">
            <div class="col-md-6 col-xs-12">
                <div class="row">
                    <div class="col-12 d-flex ">
                        <h2>Add Calification</h2>
                    </div>
                </div>
                <div class="row">
                    <div class="col-12">
                        <label class="col-12"> Name
                            <input class="input-group"/>
                        </label>
                        <label class="col-12"> Notas
                            <input class="input-group"/>
                        </label>
                    </div>
                </div>
            </div>
            <div class="col-md-6 col-xs-12">
                <div class="row">
                    <div class="col-12">
                        <div class="row">
                            <h2>Student's List</h2>
                        </div>
                        <div class="row">
                            <ul class="list-group">
                                <li v-for="item in list" :key="item.key" class="" >
                                    <span v-text="item.name" class="list-group-item mb-2"></span>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'notas',
        data: function () {
            return {
                list: [
                    { name: 'Adelys', average: '17', status: true},
                    { name: 'Jose Alberto', average: '18', status: true},
                    { name: 'Johanna', average: '17', status: true},
                    { name: 'Anna Mariet', average: '18', status: true},
                ]
            };
        },
        props: {
            msg: String
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    h3 {
        margin: 40px 0 0;
    }

    ul {
        list-style-type: none;
        padding: 0;
    }

    li {
        display: inline-block;
        margin: 0 10px;
    }

    a {
        color: #42b983;
    }
</style>
