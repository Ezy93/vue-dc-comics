<template>
    <div>
        <main>
            <section class="products">
                <div class="container">
                    content goes here
                </div>
            </section>
            <section class="main-navigation">
                <div class="container">
                    
                </div>
            </section>
        </main>
    </div>
</template>

<script>
export default {
    name: "IndexMain",
    data:function(){
        return {}
    },
    
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";

    main{
        
        section.products{
            height: 100px;
            color: white;
            background-color: black;
            
        }

        section.main-navigation{
            background-color: $brandColor;
            height: 80px;
        }
    }
</style>