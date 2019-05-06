<template>
    <nav class="navbar navbar-expand-md navbar-dark bg-dark mb-4">
        <a class="navbar-brand" href="/">书香客</a>
        <button type="button" class="navbar-toggler" data-toggle="collapse" data-target="#navbarCollapse" aria-controls="navbarCollapse" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarCollapse">
            <ul class="navbar-nav mr-auto">
                <li v-for="menu in menuList">
                    <a class="nav-item" :href="menu.url">{{ menu.name }}</a>
                </li>
            </ul>
        </div>
    </nav>
</template>

<script>
    export default {
        name: 'Navigation',
        data () {
            return {
                menuList: [
                    {name:'首页',url:'/'},
                    {name:'言情',url:'/yq'},
                    {name:'玄幻',url:'/xh'},
                    {name:'都市',url:'/ds'},
                    {name:'悬疑',url:'/xy'},
                    {name:'武侠',url:'/wx'},
                    {name:'穿越',url:'/cy'}
                ]
            }
        }
    }
</script>

<style>
    h1, h2 {
        font-weight: normal;
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
