<template>
    <div>
        <div class="content">
            <h2 class="content-title">{{titles[currentIndex]}}</h2>
            <p class="blog-content">
{{blogs[currentIndex]}}
            </p>
        </div>
<div class="buttons">
    <button @click="scrollBlogprev()" class="prev">Previous</button>
    <button @click="scrollBlognext()" class="next">Next</button>
</div>

    </div>
</template>

<script>
export default {
    name:'contents',

    data() {
        return{
            blogs:[
                "1.Lorem, ipsum dolor sit amet consectetur adipisicing elit. Fugiat doloremque impedit repudiandae! Unde quas explicabo asperiores quo voluptatem pariatur iste qui itaque quasi nisi, adipisci harum assumenda maxime officia illo.Lorem, ipsum dolor sit amet consectetur adipisicing elit. Fugiat doloremque impedit repudiandae! Unde quas explicabo asperiores quo voluptatem pariatur iste qui itaque quasi nisi, adipisci harum assumenda maxime officia illo Lorem ipsum dolor sit amet consectetur adipisicing elit. Fugiat voluptate, inventore eius velit deserunt rerum! Aperiam, perspiciatis. Omnis perferendis, ex praesentium, nobis sequi quos accusamus dignissimos distinctio veritatis dicta quam!Lorem ipsum dolor sit, amet consectetur adipisicing elit. Distinctio aut magnam magni ea maxime quam aliquid excepturi sunt doloribus hic architecto est, quibusdam optio id impedit molestias. Veritatis, est temporibus? ",
                "2.Lorem, ipsum dolor sit amet consectetur adipisicing elit. Fugiat doloremque impedit repudiandae! Unde quas explicabo asperiores quo voluptatem pariatur iste qui itaque quasi nisi, adipisci harum assumenda maxime officia illo.Lorem, ipsum dolor sit amet consectetur adipisicing elit. Fugiat doloremque impedit repudiandae! Unde quas explicabo asperiores quo voluptatem pariatur iste qui itaque quasi nisi, adipisci harum assumenda maxime officia illo Lorem ipsum dolor sit amet consectetur adipisicing elit. Fugiat voluptate, inventore eius velit deserunt rerum! Aperiam, perspiciatis. Omnis perferendis, ex praesentium, nobis sequi quos accusamus dignissimos distinctio veritatis dicta quam!Lorem ipsum dolor sit, amet consectetur adipisicing elit. Distinctio aut magnam magni ea maxime quam aliquid excepturi sunt doloribus hic architecto est, quibusdam optio id impedit molestias. Veritatis, est temporibus? ",
                "3.Lorem, ipsum dolor sit amet consectetur adipisicing elit. Fugiat doloremque impedit repudiandae! Unde quas explicabo asperiores quo voluptatem pariatur iste qui itaque quasi nisi, adipisci harum assumenda maxime officia illo.Lorem, ipsum dolor sit amet consectetur adipisicing elit. Fugiat doloremque impedit repudiandae! Unde quas explicabo asperiores quo voluptatem pariatur iste qui itaque quasi nisi, adipisci harum assumenda maxime officia illo Lorem ipsum dolor sit amet consectetur adipisicing elit. Fugiat voluptate, inventore eius velit deserunt rerum! Aperiam, perspiciatis. Omnis perferendis, ex praesentium, nobis sequi quos accusamus dignissimos distinctio veritatis dicta quam!Lorem ipsum dolor sit, amet consectetur adipisicing elit. Distinctio aut magnam magni ea maxime quam aliquid excepturi sunt doloribus hic architecto est, quibusdam optio id impedit molestias. Veritatis, est temporibus? ",
                "4.Lorem, ipsum dolor sit amet consectetur adipisicing elit. Fugiat doloremque impedit repudiandae! Unde quas explicabo asperiores quo voluptatem pariatur iste qui itaque quasi nisi, adipisci harum assumenda maxime officia illo.Lorem, ipsum dolor sit amet consectetur adipisicing elit. Fugiat doloremque impedit repudiandae! Unde quas explicabo asperiores quo voluptatem pariatur iste qui itaque quasi nisi, adipisci harum assumenda maxime officia illo Lorem ipsum dolor sit amet consectetur adipisicing elit. Fugiat voluptate, inventore eius velit deserunt rerum! Aperiam, perspiciatis. Omnis perferendis, ex praesentium, nobis sequi quos accusamus dignissimos distinctio veritatis dicta quam!Lorem ipsum dolor sit, amet consectetur adipisicing elit. Distinctio aut magnam magni ea maxime quam aliquid excepturi sunt doloribus hic architecto est, quibusdam optio id impedit molestias. Veritatis, est temporibus? "
            ],
            currentIndex:0,
            titles:[
                'Welcome To My Blog',
                'First Entry',
                'Second Entry',
                'Third Entry'
            ]
        }
    },

    methods:{
        scrollBlognext() {
this.currentIndex++;

            if(this.currentIndex >this.blogs.length - 1){
this.currentIndex = 0
            }
          
        },

        scrollBlogprev() {
this.currentIndex--;

 if(this.currentIndex < 0){
this.currentIndex= this.blogs.length-1
            }
           
        } 


    }
}
</script>

<style  scoped>
*{
    margin:0;
    padding: 0;
    box-sizing: border-box;
    font-family: sans-serif;
}

.content{
    margin-top: 20px;
    margin-left: 5%;
    margin-right: 5%;
}

.content-title{
    text-align: center;
    padding:10px 20px;
    margin-bottom: 10px;
}

.blog-content{
    line-height: 1.8rem;
    background-color: pink;
    padding:10px 20px;
    border-radius: 10px;
}

.buttons{
    margin-top: 20px;
    display:flex;
    justify-content: space-between;
}

.buttons button{
    width:10%;
    padding:5px 8px;
    background-color: black;
    color:#e75480;
    outline: none;
    border:none;
}
</style>