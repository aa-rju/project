<template>
    <template-view>
      <navbar-component></navbar-component>
  
      <!-- Section 1: Hero Section -->
      <section class="hero">
        <div class="container">
          <div class="hero-content">
            <h1>Explore Our Courses</h1>
            <p>Take your IT skills to the next level with our comprehensive training programs.</p>
            <a href="#" class="btn btn-primary">Get Started</a>
          </div>
        </div>
      </section>
  
      <!-- Section 2: Featured Courses -->
      <section class="py-5" style="background-color: #f8f8f8;" >
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
<!--       
      <section class="featured-courses">
        <div class="container">
          <h2 class="section-title">Featured Courses</h2>
          <div class="course-cards">
            <div class="course-card">
              <img src="course1.jpg" alt="Course 1">
              <h3>Course 1</h3>
              <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
              <a href="#" class="btn btn-secondary">Learn More</a>
            </div>
            <div class="course-card">
              <img src="https://pixabay.com/link/?ua=cd3%3Dimage%26cd7%3Den%253Atraining%253ANPL%26ec%3Dapi_ad%26ea%3Dnavigate%26el%3Dgetty%26tid%3DUA-20223345-1%26dr%3Dhttps%253A%252F%252Fpixabay.com%252F&sp=%2524%3Dadvertisement_clicked%26user_action%3Dnavigate%26ad_partner%3Dgetty%26ad_content%3Dapi_ad%26ad_type%3D%26media_type%3Dphoto%26media_subtype%3D%26media_id%3D&next=https%3A%2F%2Fwww.istockphoto.com%2Fphoto%2Fyoung-happy-woman-student-using-laptop-watching-webinar-writing-at-home-gm1446806057-484783204%3Futm_source%3Dpixabay%26utm_medium%3Daffiliate%26utm_campaign%3DSRP_image_sponsored%26utm_content%3Dhttps%253A%252F%252Fpixabay.com%252Fimages%252Fsearch%252Ftraining%252F%26utm_term%3Dtraining&hash=e2ff5b4a19e5d96b9ca3c72fb1e0dabcb44f0d5c&=" alt="Course 2">
              <h3>Course 2</h3>
              <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
              <a href="#" class="btn btn-secondary">Learn More</a>
            </div>
            <div class="course-card">
              <img src="https://pixabay.com/link/?ua=cd3%3Dimage%26cd7%3Den%253Atraining%253ANPL%26ec%3Dapi_ad%26ea%3Dnavigate%26el%3Dgetty%26tid%3DUA-20223345-1%26dr%3Dhttps%253A%252F%252Fpixabay.com%252F&sp=%2524%3Dadvertisement_clicked%26user_action%3Dnavigate%26ad_partner%3Dgetty%26ad_content%3Dapi_ad%26ad_type%3D%26media_type%3Dphoto%26media_subtype%3D%26media_id%3D&next=https%3A%2F%2Fwww.istockphoto.com%2Fphoto%2Fsenior-business-woman-holding-presentation-gm1385520247-444236122%3Futm_source%3Dpixabay%26utm_medium%3Daffiliate%26utm_campaign%3DSRP_image_sponsored%26utm_content%3Dhttps%253A%252F%252Fpixabay.com%252Fimages%252Fsearch%252Ftraining%252F%26utm_term%3Dtraining&hash=4b508e67598cfa58895d0faa45d5d7dec6d64752&=" alt="Course 3">
              <h3>Course 3</h3>
              <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
              <a href="#" class="btn btn-secondary">Learn More</a>
            </div>
          </div>
        </div>
      </section> -->
  
      <!-- Section 3: Testimonials -->
      <section class="testimonials animate-up">
        <div class="container">
          <h2 class="section-title">Student Testimonials</h2>
          <div class="testimonial-slider">
            <div class="testimonial-slide">
              <img src="avatar1.jpg" alt="Avatar 1">
              <p>"Lorem ipsum dolor sit amet, consectetur adipiscing elit."</p>
              <h4>John Doe</h4>
            </div>
            <div class="testimonial-slide">
              <img src="avatar2.jpg" alt="Avatar 2">
              <p>"Lorem ipsum dolor sit amet, consectetur adipiscing elit."</p>
              <h4>Jane Smith</h4>
            </div>
          </div>
        </div>
      </section>
  
      <!-- Section 4: Upcoming Courses -->
      <section class="upcoming-courses animate-up">
        <div class="container">
          <h2 class="section-title">Upcoming Courses</h2>
          <div class="course-list">
            <div class="course-item">
              <img src="course4.jpg" alt="Course 4">
              <div class="course-details">
                <h3>Course 4</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
                <a href="#" class="btn btn-secondary">Learn More</a>
              </div>
            </div>
            <div class="course-item">
              <img src="course5.jpg" alt="Course 5">
              <div class="course-details">
                <h3>Course 5</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
                <a href="#" class="btn btn-secondary">Learn More</a>
              </div>
            </div>
            <div class="course-item">
              <img src="course6.jpg" alt="Course 6">
              <div class="course-details">
                <h3>Course 6</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
                <a href="#" class="btn btn-secondary">Learn More</a>
              </div>
            </div>
          </div>
        </div>
      </section>
  
      <!-- Section 5: Call to Action -->
      <section class="cta animate-up">
        <div class="container">
          <h2 class="section-title">Ready to Take the Next Step?</h2>
          <p>Enroll in our courses today and boost your IT career.</p>
          <a href="#" class="btn btn-primary">Enroll Now</a>
        </div>
      </section>
    </template-view>
  </template>
  
  <script>
  import TemplateView from './TemplateView.vue';
  import NavbarComponent from '@/components/NavbarComponent.vue';
  import CardComponent from '@/components/CardComponent.vue';
  
  export default {
    mounted() {
    // Attach scroll event listener when the component is mounted
    window.addEventListener('scroll', this.handleScroll);
  },

  destroyed() {
    // Remove scroll event listener when the component is destroyed
    window.removeEventListener('scroll', this.handleScroll);
  },
    components: { TemplateView, NavbarComponent,CardComponent },
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
  };
  
  </script>
  
  <style scoped>
  /* General Styles */
  .container {
    max-width: 1200px;
    margin: 0 auto;
  }
  
  .section-title {
    text-align: center;
    margin-bottom: 40px;
  }
  
  .btn {
    display: inline-block;
    padding: 10px 20px;
    border-radius: 4px;
    font-size: 16px;
    text-decoration: none;
    text-align: center;
    transition: background-color 0.3s ease;
  }
  
  .btn-primary {
    background-color: black;
    color: #fff;
  }
  
  .btn-secondary {
    background-color: #6c757d;
    color: #fff;
  }
  
  /* Hero Section */
  .hero {
    background-color: rgba(188, 150, 110, 0.936);
    padding: 100px 0;
  }
  
  .hero-content {
    text-align: center;
  }
  
  /* Featured Courses Section */
  .featured-courses {
    padding: 80px 0;
  }
  
  /* Featured and Upcoming Courses Animation */
.course-card,
.course-item {
  position: relative;
  overflow: hidden;
  transition: transform 0.3s;
}

.course-card:hover,
.course-item:hover {
  transform: translateY(-5px);
}

.course-card::before,
.course-item::before {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.3);
  opacity: 0;
  z-index: 1;
  transition: opacity 0.3s;
}

.course-card:hover::before,
.course-item:hover::before {
  opacity: 1;
}

.course-card:hover img,
.course-item:hover img {
  transform: scale(1.1);
}

  
  /* Testimonials Section */
  .testimonials {
    background-color: #f8f9fa;
    padding: 80px 0;
  }
  
  .testimonial-slider {
    display: flex;
    justify-content: center;
    gap: 30px;
  }
  
  .testimonial-slide {
    max-width: 400px;
    text-align: center;
  }
  
  .testimonial-slide img {
    width: 100px;
    height: 100px;
    border-radius: 50%;
    margin-bottom: 20px;
  }
  
  /* Upcoming Courses Section */
  .upcoming-courses {
    padding: 80px 0;
  }
  
  .course-list {
    display: flex;
    justify-content: center;
    gap: 30px;
  }
  
  .course-item {
    display: flex;
    align-items: center;
    max-width: 600px;
  }
  
  .course-item img {
    width: 150px;
    height: auto;
    margin-right: 20px;
  }
  
  /* Call to Action Section */
  .cta {
    background-color:  rgba(188, 150, 110, 0.936);
    padding: 80px 0;
    text-align: center;
  }
  
  .cta p {
    color: #fff;
    margin-bottom: 40px;
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
