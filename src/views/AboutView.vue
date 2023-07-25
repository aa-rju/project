<template>
  <template-view>
    <navbar-component></navbar-component>

    <section class=" py-5 " style="background-color: #FFF8E5; margin-top: 40px;">
      <div class="container">
        <h1>About Us</h1>
        <!-- About Us content -->
        <p><b>Welcome to our IT Training Center, where we strive to empower individuals with the knowledge and skills needed to excel in the field of Information Technology.</b></p>
        <br><p>At our center, we are passionate about providing high-quality training programs that cater to both beginners and professionals seeking to enhance their IT skills. With experienced instructors and a comprehensive curriculum, we ensure a conducive learning environment for all our students.</p>
        <p>Our mission is to bridge the gap between academia and industry by equipping our students with practical IT skills that are in high demand in today's job market. We are committed to fostering a culture of continuous learning and professional development.</p>
        <p>Whether you are looking to kick-start your IT career, upskill in a specific area, or stay updated with the latest technologies, our training center offers a wide range of courses and certifications to meet your needs. Our courses cover topics such as programming, web development, cybersecurity, database management, cloud computing, and more.</p>
        <p>We pride ourselves on our experienced and knowledgeable instructors who are industry experts and passionate educators. They bring real-world experience and insights into the classroom, ensuring that our students receive practical, up-to-date knowledge that can be immediately applied in their careers.</p>
      </div>
    </section>

    <!-- Other sections... -->

    <!-- Blogs section with animation -->
    <section class="py-5 animate-up" style="background-color: #FCE38A; margin-top: 40px;">
      <div class="container">
        <h2>Check out Blogs</h2>
        <div class="row">
          <div v-for="blog in blogs" :key="blog.id" class="col-md-4">
            <div class="blog-card animate">
              <img :src="blog.image" alt="Blog Image" class="blog-image">
              <h3>{{ blog.title }}</h3>
              <p>{{ blog.description }}</p>
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

export default {
  mounted() {
      // Attach scroll event listener when the component is mounted
      window.addEventListener('scroll', this.handleScroll);
    },
  
    destroyed() {
      // Remove scroll event listener when the component is destroyed
      window.removeEventListener('scroll', this.handleScroll);
    },
  components: {
    TemplateView,
    NavbarComponent,
  },
  methods: {
    handleScroll() {
      // Get the elements with the animate-up class
      const elements = document.querySelectorAll('.animate-up');

      // Loop through the elements and check if they are in the viewport
      elements.forEach((element) => {
        const rect = element.getBoundingClientRect();

        // If the element is in the viewport, add a CSS class to trigger the animation
        if (rect.top <= window.innerHeight * 0.75) {
          element.classList.add('animate');
        } else {
          // If the element is not in the viewport, remove the CSS class
          element.classList.remove('animate');
        }
      });
    },
  },
  data() {
    return {
      blogs: [
        {
          id: 1,
          title: "Blog 1",
          description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
          image: "blog1.jpg",
        },
        {
          id: 2,
          title: "Blog 2",
          description: "Nullam sit amet fermentum orci, sed interdum ligula.",
          image: "blog2.jpg",
        },
        {
          id: 3,
          title: "Blog 3",
          description: "Nunc sollicitudin massa nec risus varius, ac aliquet ipsum aliquet.",
          image: "blog3.jpg",
        },
      ],
    };
  },
}
</script>

<style scoped>
.animate {
  animation: blogAnimation 1s ease-in-out infinite alternate;
}

@keyframes blogAnimation {
  0% {
    transform: translateY(0);
  }
  100% {
    transform: translateY(-10px);
  }
}

.blog-card {
  background-color: #fff;
  border-radius: 5px;
  padding: 20px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
  margin-bottom: 20px;
  text-align: center;
}

.blog-image {
  width: 100%;
  height: auto;
  object-fit: cover;
  border-radius: 5px;
  margin-bottom: 10px;
}

.blog-card h3 {
  font-size: 18px;
  margin-bottom: 10px;
}

.blog-card p {
  margin-bottom: 5px;
}
.animate-up {
  animation: slideInUp 2s ease-in-out;
}
.animate-up {
  opacity: 0;
  transform: translateX(-100%);
  transition: opacity 1s ease, transform 1s ease;
}

.animate {
  opacity: 1;
  transform: translateX(0);
}
</style>
