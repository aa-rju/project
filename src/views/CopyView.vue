

<!-- <template>
  <template-view>
    <navbar-component></navbar-component>
    
    <section class="py-5">
      <div class="container">
        <h6 class="custom-heading">Explore our new courses by signing in and stay up-to-date with us</h6>
      </div>
    </section>
    
    <!-- section1 -->
    <section class="py-4">
      <div class="container">
        <div class="row">
          <div class="col-md-8"><carousel-component/></div>
          <div class="col-md-4"><p class="typewriter"><br><br><br><b>The website will serve as an online platform to showcase training programs and various courses.

IT training center will provide a user-friendly interface for potential students to explore, register, and participate in these programs.

These website will play a crucial role in attracting prosperous students.

It utilizes various digital tools to deliver content and facilitate interactive learning experiences.</b>
</p></div>
        </div>
      </div>
    </section>

    <!-- section2 -->
    <section class="py-5" style="background-color: #d6da7b;" >
      <div class="container">
        <h4>Our Learning Library</h4>
        <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Ullam, dolor ab quibusdam, provident voluptate nemo sapiente quis exercitationem, cum at sint reprehenderit ipsam. Suscipit nesciunt veritatis nobis. Ipsum, laboriosam corrupti!</p>
        <div class="row">
          <div class="col-md-3">
            <card-component></card-component>
          </div>
          <div class="col-md-3">
            <card-component></card-component>
          </div>
          <div class="col-md-3">
            <card-component></card-component>
          </div>
          <div class="col-md-3">
            <card-component></card-component>
          </div>
        </div>
        <div class="row py-3">
          <div class="col-md-3">
            <card-component></card-component>
          </div>
          <div class="col-md-3">
            <card-component></card-component>
          </div>
          <div class="col-md-3">
            <card-component></card-component>
          </div>
          <div class="col-md-3">
            <card-component></card-component>
          </div>
        </div>
      </div>
    </section>

    <!-- section4 -->
    <section class="py-5" style="background-color: #cccdb9; margin-top: 40px;">
      <h2>Blogs</h2>
      <div class="container py-2">
        <div class="row mx-auto">
          <div class="col-md-4"><blog-component></blog-component></div>
          <div class="col-md-4"><blog-component></blog-component></div>
          <div class="col-md-4"><blog-component></blog-component></div>
        </div>
      </div>
    </section>

    <!-- section5 -->
    <section class="py-5 tutor-section" style="background-color: #d6da7b; margin-top: 40px;">
  <div class="container">
    <h2>Tutors</h2>
    <div class="row">
      <div class="col-md-4">
        <div class="tutor-card animate">
          <div class="tutor-image-container">
            <img src="tutor1.jpg" alt="Tutor 1" class="tutor-image">
          </div>
          <!-- <h3>Tutor 1</h3> -->
          <p>Degree: </p>
          <p>Expertise: </p>
        </div>
      </div>
      <div class="col-md-4">
        <div class="tutor-card animate">
          <div class="tutor-image-container">
            <img src="tutor2.jpg" alt="Tutor 2" class="tutor-image">
          </div>
          <!-- <h3>Tutor 2</h3> -->
          <p>Degree: </p>
          <p>Expertise: </p>
        </div>
      </div>
      <div class="col-md-4">
        <div class="tutor-card animate">
          <div class="tutor-image-container">
            <img src="tutor3.jpg" alt="Tutor 3" class="tutor-image">
          </div>
          <!-- <h3>Tutor 3</h3> -->
          <p>Degree:</p>
          <p>Expertise: </p>
        </div>
      </div>
    </div>
  </div>
</section>

  </template-view>
</template>

<script>
import TemplateView from './TemplateView.vue';
import NavbarComponent from '@/components/NavbarComponent.vue';
import CarouselComponent from '@/components/CarouselComponent.vue';
import CardComponent from '@/components/CardComponent.vue';
import BlogComponent from '@/components/BlogComponent.vue';

export default {
  components: {
    TemplateView,
    NavbarComponent,
    CarouselComponent,
    CardComponent,
    BlogComponent,
  },
}
</script>

<style scoped>
.client-logo-img {
  position: relative;
  left: calc(50% - 50px);
  animation: slideAnimation 4s linear infinite;
}

@keyframes slideAnimation {
  0% {
    left: calc(50% - 50px);
  }
  20% {
    left: calc(25% - 50px);
  }
  80% {
    left: calc(75% - 50px);
  }
  100% {
    left: calc(50% - 50px);
  }
}

.custom-heading {
  color: rgba(211, 147, 18, 0.87);
  background-color: black;
  animation: myAnimation 2s infinite;
}

@keyframes myAnimation {
  0% { transform: scale(1); }
  50% { transform: scale(1.2); }
  100% { transform: scale(1); }
}
.animate {
  animation: tutorAnimation 1s ease-in-out infinite alternate;
}

@keyframes tutorAnimation {
  0% {
    transform: translateY(0);
  }
  100% {
    transform: translateY(-10px);
  }
}

.tutor-card {
  background-color: #fff;
  border-radius: 5px;
  padding: 20px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
  margin-bottom: 20px;
  text-align: center;
}

.tutor-image-container {
  width: 120px;
  height: 120px;
  border-radius: 50%;
  overflow: hidden;
  margin: 0 auto 10px;
}

.tutor-image {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

</style> -->