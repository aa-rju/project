<template>
    <template-view>
        <navbar-component class="py-5"></navbar-component>
        <div>
      <!-- <section class="py-3 first-section">
        <div class="carousel-container">
          <div class="carousel-text">Welcome to Our Website</div>
          <carousel-component></carousel-component>
        </div>
      </section> -->
      <!-- section1 -->
    <section class="py-5" style="background-color: rgb(237, 222, 222);">
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
  
      <section class=" py-3 contact-section animate-up">
        <h2 class="title">Contact Us</h2>
        <p class="description">If you have any queries, please do not hesitate to contact us.</p>
        <div class="contact-info">
          <div class="contact-item-box" v-for="(item, index) in contactItems" :key="index">
            <div class="contact-item">
              <div class="contact-item-icon">
                <i class="fas" :class="item.icon"></i>
              </div>
              <div class="contact-item-content">
                <p class="contact-label">{{ item.label }}:</p>
                <p class="contact-value">{{ item.value }}</p>
              </div>
            </div>
          </div>
        </div>
      </section>
      </div>
  
      <section class="social-section animate-up">
        <h2 class="title">We Are On</h2>
        <div class="social-links">
          <a href="https://www.facebook.com" target="_blank" rel="noopener" class="social-link facebook">
            <i class="fab fa-facebook"></i>
          </a>
          <a href="https://www.instagram.com" target="_blank" rel="noopener" class="social-link instagram">
            <i class="fab fa-instagram"></i>
          </a>
          <a href="https://www.linkedin.com" target="_blank" rel="noopener" class="social-link linkedin">
            <i class="fab fa-linkedin"></i>
          </a>
        </div>
      </section>
  
      <section class="enroll-section animate-up">
      <h2 class="title">Enroll Now</h2>
      <p class="description">Fix your seat making a payment:</p>
      <div class="payment-options">
        <div class="payment-option">
          <div class="payment-icon">
            <img src="bank_account_qr_code.png" alt="Bank Account QR Code">
          </div>
          <div class="payment-details">
            <p class="payment-label">Bank Transfer</p>
            <p class="payment-value">Account Number: 123456789</p>
          </div>
        </div>
      </div>
    </section>
    </template-view>
  </template>
  
  <script>
  import CarouselComponent from '@/components/CarouselComponent.vue';
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


    name: 'ContactView',
    components: {
      CarouselComponent,
        TemplateView,
        NavbarComponent
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
        contactItems: [
          { icon: 'fa-envelope', label: 'Email', value: 'mahataaarju@gmail.com' },
          { icon: 'fa-phone', label: 'Call Us', value: '9848770282' },
          { icon: 'fa-map-marker-alt', label: 'Address', value: 'Sampang street,Dharan, Nepal' }
        ]
      };
    }
  }
  
  </script>
  
  <style scoped>
  .first-section {
    background-color: #FCE38A;
    color: #000;
    padding: 40px;
    /* Add styling for the first section with carousel */
  }
  .first-section {
  background-color: #FCE38A;
  color: #000;
  padding: 0;
  overflow: hidden;
}

.carousel-container {
  max-width: 100%;
  height: 100vh; /* Set the height of the carousel container to fit the screen */
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.carousel-text {
  font-size: 24px;
  font-weight: bold;
  margin-bottom: 20px;
}
  
  .contact-section {
    background-color: #FFF8E5;
    color: #000;
    padding: 40px;
  }
  
  .title {
    font-size: 28px;
    font-weight: bold;
    margin-bottom: 20px;
  }
  
  .description {
    font-size: 18px;
  }
  
  .contact-info {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
  }
  
  .contact-item-box {
    background-color: #FFEDC2;
    border-radius: 10px;
    padding: 20px;
    margin: 10px;
  }
  
  .contact-item {
    display: flex;
    align-items: center;
    margin-bottom: 10px;
  }
  
  .contact-item-icon {
    margin-right: 10px;
  }
  
  .contact-label {
    font-size: 16px;
    margin-bottom: 5px;
  }
  
  .contact-value {
    font-size: 16px;
  }
  
  .social-section {
    background-color: #FCE38A;
    color: #000;
    padding: 40px;
  }
  
  .social-links {
    display: flex;
    justify-content: center;
  }
  
  .social-link {
    color: #000;
    font-size: 24px;
    margin: 0 10px;
    transition: color 0.3s ease;
  }
  
  .social-link:hover {
    color: #FFEDC2;
  }
  
  .additional-section {
    background-color: #FFF8E5;
    color: #000;
    padding: 40px;
  }
  .first-section {
  background-color: #FCE38A;
  color: #000;
  padding: 40px;
}

.carousel-container {
  max-width: 100%;
  overflow: hidden;
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
  
  