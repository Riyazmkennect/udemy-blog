<template>
  <div class="home-page">
    <section class="intro">
      <h1 >Get the latest tech News!</h1>
    </section>
    <!-- <section class="featured-posts">
      <nuxt-link :to=" '/posts/' + 1" class="post-preview">
      <article>
         <div class="post-thumbnail" style="background-image: url('https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT37yDMnk58NLCu5-DactqepKxNIEHyG7tS_A&usqp=CAU')"></div>
         <div class="post-content"></div>
         <h1>post Title 1</h1>
         <p> Text title 1</p>
      </article>
      </nuxt-link>
        <nuxt-link :to=" '/posts/' + 2" class="post-preview">
      <article >
         <div class="post-thumbnail" style="background-image: url('https://images.pexels.com/photos/1193743/pexels-photo-1193743.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1')"></div>
         <div class="post-content"></div>
         <h1>post Title 2</h1>
         <p> Text title 2</p>
      </article>
      </nuxt-link>
   </section> -->
    <section class="featured-posts">
      <PostPreview 
      id="1"
      title="dubai designs"
      thumbnail="https://images.pexels.com/photos/1193743/pexels-photo-1193743.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"
     PreviewText=" ann uhibhukka"
      />
       <PostPreview 
      id="1"
      title="dubai designs"
      thumbnail="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSLYCT99EjTNQX-LkfXrOtY_vQEZWaq6YdQM_WFYBpD7e5DG3fwn99M87Cc2QqfFhM6D-s&usqp=CAU"
     PreviewText=" ann uhibhukka"
      />
       <PostPreview 
      id="1"
      title="dubai designs"
      thumbnail="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRp0-c7PZi3hJulH_fnbH3UfG_4iX6ULwsuKQ&usqp=CAU"
     PreviewText=" ann uhibhukka"
      />
       <PostPreview 
      id="1"
      title="dubai designs"
      thumbnail="https://images.pexels.com/photos/1193743/pexels-photo-1193743.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"
     PreviewText=" ann uhibhukka"
      />
       <PostPreview 
      id="1"
      title="dubai designs"
      thumbnail="https://media.tycsports.com/files/2021/12/13/371380/lionel-messi-dubai_862x485.jpg?v=1"
     PreviewText=" ann uhibhukka"
      />
       <PostPreview 
      id="1"
      title="dubai designs"
      thumbnail="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSPloSSiJwtUdUsyzju59xEslsT_A7g3VskdzPkx5oeElUXhQaGTH0sOmy3fdAkqXbJnRQ&usqp=CAU"
     PreviewText=" ann uhibhukka"
      />
       <PostPreview 
      id="1"
      title="dubai designs"
      thumbnail="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQYARhSLzv2S2C-CiV4SCsKHBD-t4wVWc--hA&usqp=CAU"
      />

    
    </section>
  </div>
</template>

<script>
import PostPreview from "../components/posts/PostPreview.vue";
export default {
  name: "IndexPage",
  components: {
    PostPreview,
  },
};
</script>
<style scoped>
.intro {
  height: 300px;
  position: relative;
  padding: 30px;
  box-sizing: border-box;
  background-image: url('~assets/images/dubai.jpg');
  background-position: center;
  background-size: cover;

}

.intro h1 {
  position: absolute;
  top: 10%;
  left: 5%;
  width: 90%;
  font-size: 1.5rem;
  color: black;
  background-color: rgb(211, 211, 211);
  padding: 10px;
  border-radius: 10px;
  box-shadow: 3px 3px 3px black;
  box-sizing: border-box;
  border: 1px solid black;
}

@media (min-width: 768px) {
  .intro h1 {
    font-size: 2rem;
  }
}

.featured-posts {
  display: flex;
  padding: 40px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
  width: 100%;
}

.post-preview {
  border: 1px solid #ccc;
  box-shadow: 0 2px 2px #ccc;
  background-color: white;
  width: 90%;
}

a {
  text-decoration: none;
  color: black;
}

@media (min-width: 850px) {
  .post-preview {
    width: 400px;
    margin: 10px;
  }
}

.post-thumbnail {
  width: 100%;
  height: 200px;
  background-position: center;
  background-size: cover;
}

.post-content {
  padding: 10px;
  text-align: center;
}

a:hover .post-content,
a:active .post-content {
  background-color: #ccc;
}
.hav h1{
  align-content: center;
  
}
</style>