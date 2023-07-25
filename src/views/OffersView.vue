<template>
    <template-view>
      <navbar-component></navbar-component>
  
      <!-- Section 1: Hero Section -->
      <section class="hero">
        <div class="container">
          <div class="hero-content">
            <h1>Special Offers</h1>
            <p>Check out our latest offers and promotions.</p>
          </div>
        </div>
      </section>
  
      <!-- Section 2: Offer Cards -->
      <section class="offer-cards" >
        <div class="container">
          <div class="card-grid">
            <div class="offer-card">
              <img src="https://media.istockphoto.com/id/1383431114/photo/ux-designer-planning-application-for-mobile-phone.webp?b=1&s=612x612&w=0&k=20&c=3f5an9KsYhNXtzK8t8DwPvRjGLLGu5_QaQmSu2pR3D8=" alt="Offer 1">
              <h3>Web development</h3>
              <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
              <a href="#" class="btn btn-primary">Learn More</a>
            </div>
            <div class="offer-card">
              <img src="https://media.istockphoto.com/id/1174690086/photo/software-developer-freelancer-working-at-home.jpg?s=1024x1024&w=is&k=20&c=6d1JmwVhkUv6whYZbDHXpGSnYicvS85Uj1o1YTH05h4=" alt="Offer 2">
              <h3>Flutter:app development</h3>
              <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
              <a href="#" class="btn btn-primary">Learn More</a>
            </div>
            <div class="offer-card">
              <img src="https://media.istockphoto.com/id/1056564406/photo/graphic-designer-drawing-on-graphics-tablet-at-workplace.jpg?s=612x612&w=0&k=20&c=w_ZE4TKsB5DtjZOrwjO29VNx5THaZvvAzoBR2JSz6sY=" alt="Offer 3">
              <h3>Graphics Design</h3>
              <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
              <a href="#" class="btn btn-primary">Learn More</a>
            </div>
          </div>
        </div>
      </section>
  
      <!-- Section 3: Call to Action -->
      <section class="cta animate-up">
        <div class="container">
          <h2 class="section-title">Don't Miss Out!</h2>
          <p>Take advantage of these limited-time offers today.</p>
          <div class="contact-info">
            <div class="contact-item">
              <i class="fas fa-envelope"></i>
              <a href="mailto:info@example.com">info@example.com</a>
            </div>
            <div class="contact-item">
              <i class="fas fa-phone"></i>
              <a href="tel:+1234567890">+1234567890</a>
            </div>
            <div class="contact-social">
              <a href="https://www.facebook.com" target="_blank"><i class="fab fa-facebook"></i></a>
              <a href="https://www.instagram.com" target="_blank"><i class="fab fa-instagram"></i></a>
              <a href="https://www.linkedin.com" target="_blank"><i class="fab fa-linkedin"></i></a>
            </div>
          </div>
          <a href="#" class="btn btn-primary">Get Started</a>
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
    components: { TemplateView, NavbarComponent },
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
}

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
    background-color: rgb(5, 5, 4);
    color: #f8f8f8;
  }
  
  /* Hero Section */
  .hero {
    background-color: #000;
    padding: 100px 0;
  }
  
  .hero-content {
    text-align: center;
  }
  
  .hero-content h1,
  .hero-content p {
    color: #fff;
  }
  
  /* Offer Cards Section */
  .offer-cards {
    padding: 80px 0;
    background-color: rgba(240, 236, 231, 0.936);
  }
  
  .card-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 30px;
  }
  
  .offer-card {
    text-align: center;
    background-color: rgba(188, 150, 110, 0.936);
    padding: 30px;
    border-radius: 8px;
  }
  
  .offer-card img {
    width: 100%;
    height: auto;
    margin-bottom: 20px;
  }
  
  .offer-card h3 {
    color: black;
  }
  
  .offer-card p {
    color: #777;
  }
  
  /* Call to Action Section */
  .cta {
    background-color: #adaca9;
    padding: 80px 0;
    text-align: center;
  }
  
  .cta p {
    color: #000;
    margin-bottom: 20px;
  }
  
  .contact-info {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 20px;
    margin-bottom: 30px;
  }
  
  .contact-item a {
    color: #000;
    text-decoration: none;
  }
  
  .contact-social a {
    color: #000;
    text-decoration: none;
    font-size: 24px;
    margin-right: 10px;
  }
  
  /* AOS animations */
  [data-aos] {
    opacity: 0;
    transition-property: opacity;
  }
  
  [data-aos].aos-animate {
    opacity: 1;
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
  