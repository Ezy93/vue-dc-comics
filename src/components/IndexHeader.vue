<template>
    <div>
        <header>
            <nav>
                <img src="../assets/images/dc-logo.png" alt="logo dc comics">
                <ul>
                    <li v-for="(link,index) in navList" :key="index">
                        <a href="#">{{link.name}}</a>
                    </li>
                    
                </ul>
            </nav>
        </header>
    </div>
</template>

<script>
export default{
    name: 'IndexHeader',
    data:function() {
        return {
            navList: [
                {
                    name: "characters",
                    clicked: true
                },
                {
                    name: "comics",
                    clicked: true
                },
                {
                    name: "movies",
                    clicked: true
                },
                {
                    name: "tv",
                    clicked: true
                },
                {
                    name: "games",
                    clicked: true
                },
                {
                    name: "collectibles",
                    clicked: true
                },
                {
                    name: "videos",
                    clicked: true
                },
                {
                    name: "fans",
                    clicked: true
                },
                {
                    name: "news",
                    clicked: true
                },
                {
                    name: "shop",
                    clicked: true
                },
            ]
        }

        
    }
}
</script>

<style lang="scss" scoped>
    div{
        width: 80%;
        margin: 0 auto;

        nav{
            display: flex;
            justify-content: space-between;

            ul{
                display: flex;
                align-items: center;
                list-style-type: none;
                margin: 0;

                li{
                    margin: 0rem .9rem;
                    line-height: 103px;

                    a{
                        text-decoration: none;
                        color: #544F56;
                    }
                }
            }
        }
    }
</style>