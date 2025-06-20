---
layout: default
title: XOST STUDIO
description: Futuristic software and gaming brand building next-gen digital experiences
image: https://raw.githubusercontent.com/XOST-Studio/XOST-Studio.github.io/main/XostStudio.png
---

<style>
  @keyframes float {
    0%, 100% { transform: translateY(0); }
    50% { transform: translateY(-10px); }
  }
  @keyframes pulse {
    0%, 100% { box-shadow: 0 0 20px #82e85b, 0 0 30px #c1ebf2; }
    50% { box-shadow: 0 0 30px #82e85b, 0 0 40px #c1ebf2; }
  }
  @keyframes progress {
    0% { stroke-dashoffset: 314; }
    100% { stroke-dashoffset: var(--target-offset); }
  }
  .skill-circle {
    position: relative;
    width: 120px;
    height: 120px;
    margin: 0 auto;
  }
  .circle-bg {
    fill: none;
    stroke: rgba(194, 232, 242, 0.1);
    stroke-width: 8;
  }
  .circle-progress {
    fill: none;
    stroke: #82e85b;
    stroke-width: 8;
    stroke-linecap: round;
    stroke-dasharray: 314;
    transform-origin: center;
    transform: rotate(-90deg);
  }
  .neon-text {
    text-shadow: 0 0 5px #82e85b, 0 0 10px #c1ebf2;
  }
  .skills-container {
    opacity: 0;
    transition: opacity 0.5s ease, transform 0.5s ease;
    transform: translateY(20px);
  }
  .skills-container.visible {
    opacity: 1;
    transform: translateY(0);
  }
</style>

<script>
  document.addEventListener('DOMContentLoaded', function() {
    const skillsSection = document.querySelector('#skills-section');
    const observer = new IntersectionObserver((entries) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.classList.add('visible');
          // Trigger circle animations
          const circles = entry.target.querySelectorAll('.circle-progress');
          circles.forEach(circle => {
            circle.style.animation = 'progress 1.5s ease-out forwards';
          });
        }
      });
    }, { threshold: 0.1 });
    
    if (skillsSection) {
      observer.observe(skillsSection);
    }
  });
</script>


  <!-- Header -->
  <h1 style="text-align: center; color: #82e85b; font-size: 3.5rem; margin-bottom: 10px; animation: float 3s ease-in-out infinite;" class="neon-text">
    ⚡ XOST STUDIO
  </h1>
  
  <p style="text-align: center; font-size: 1.2rem; margin-bottom: 30px; animation: float 3s ease-in-out infinite 0.5s;">
    <span style="display: inline-block; background: linear-gradient(90deg, #82e85b, #c1ebf2); -webkit-background-clip: text; -webkit-text-fill-color: transparent; text-shadow: 0 0 8px rgba(194, 232, 242, 0.3);">
      👾 Welcome to the digital playground of <strong>XOST Studio</strong> — where code meets imagination.
    </span>
  </p>

  <!-- Animated Banner -->
  <div style="position: relative; margin: 30px 0;">
    <img src="https://raw.githubusercontent.com/XOST-Studio/XOST-Studio.github.io/main/XostStudio.png" alt="XOST Banner" style="width:100%; border-radius: 15px; animation: pulse 4s ease-in-out infinite; border: 1px solid rgba(194, 232, 242, 0.2);">
    <div style="position: absolute; bottom: 0; left: 0; right: 0; height: 30%; background: linear-gradient(transparent, rgba(0,0,0,0.7)); border-radius: 0 0 15px 15px;"></div>
  </div>

  <!-- About Section -->
  <section style="margin: 50px 0; position: relative;">
    <h2 style="text-align: center; font-size: 2.2rem; margin-bottom: 30px;">
      <span style="display: inline-block; background: linear-gradient(90deg, #82e85b, #c1ebf2); -webkit-background-clip: text; -webkit-text-fill-color: transparent;">
        🚀 ABOUT XOST STUDIO
      </span>
    </h2>
    <p style="font-size: 1.1rem; line-height: 1.6;">
      <strong>XOST Studio</strong> is a next-gen creative development studio focused on crafting immersive games, futuristic software, and powerful digital experiences. Founded by <strong>Muhammad Waleed</strong>, we blend hardware innovation with software excellence to push boundaries in interactive technology.
    </p>
    <div style="background: rgba(194, 232, 242, 0.1); padding: 20px; border-left: 3px solid #82e85b; border-radius: 0 10px 10px 0; margin: 30px 0; backdrop-filter: blur(5px);">
      <p style="font-size: 1.2rem; line-height: 1.6; margin: 0;">
        We're more than just developers — we're <span style="color: #82e85b;">world-builders</span>.<br>
        From <span style="color: #c1ebf2;">pixels to players</span>, <span style="color: #82e85b;">code to cosmos</span>, every project is a fusion of engineering rigor and creative vision.
      </p>
    </div>
  </section>

  <!-- Founder Section -->
  <section style="margin: 60px 0;">
    <h2 style="text-align: center; font-size: 2.2rem; margin-bottom: 30px;">
      <span style="display: inline-block; background: linear-gradient(90deg, #82e85b, #c1ebf2); -webkit-background-clip: text; -webkit-text-fill-color: transparent;">
        👨‍💻 FOUNDER & CEO
      </span>
    </h2>
    <div style="display: flex; flex-wrap: wrap; gap: 30px; align-items: center; justify-content: center; margin: 40px 0;">
      <!-- Circular Skill Graph -->
      <div style="flex: 0 0 300px;">
        <div class="skill-circle">
          <svg viewBox="0 0 120 120">
            <circle class="circle-bg" cx="60" cy="60" r="50"></circle>
            <circle class="circle-progress" cx="60" cy="60" r="50" stroke-dashoffset="78.5"></circle> <!-- 75% -->
          </svg>
          <div style="position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%); text-align: center;">
            <span style="color: #82e85b; font-size: 1.8rem; font-weight: bold;">C++</span><br>
            <span style="color: #c1ebf2;">Expert</span>
          </div>
        </div>
      </div>
      <div style="flex: 1; min-width: 300px;">
        <h3 style="margin-top: 0; color: #c1ebf2; font-size: 1.8rem;">
          <span style="color: #82e85b;">MUHAMMAD WALEED</span>
        </h3>
        <div style="display: flex; gap: 10px; flex-wrap: wrap; margin: 15px 0;">
          <span style="background: rgba(130, 232, 91, 0.2); padding: 5px 12px; border-radius: 20px; border: 1px dashed #82e85b; animation: float 3s ease-in-out infinite 1s;">Electrical Engineer</span>
          <span style="background: rgba(194, 232, 242, 0.2); padding: 5px 12px; border-radius: 20px; border: 1px dashed #c1ebf2; animation: float 3s ease-in-out infinite 1.2s;">Embedded Systems</span>
          <span style="background: rgba(130, 232, 91, 0.2); padding: 5px 12px; border-radius: 20px; border: 1px dashed #82e85b; animation: float 3s ease-in-out infinite 1.4s;">Creative Technologist</span>
        </div>
        <div style="color: #c1ebf2; margin: 20px 0; font-size: 1.1rem;">
          📍 Lahore, Pakistan | ✉️ waleednaeem133@gmail.com | 🔗 
          <a href="https://github.com/W-N-R" style="color: #82e85b; text-decoration: none; transition: all 0.3s;" onmouseover="this.style.textShadow='0 0 5px #82e85b'" onmouseout="this.style.textShadow='none'">GitHub</a>
        </div>
        <div style="background: rgba(194, 232, 242, 0.05); padding: 15px; border-radius: 10px; border: 1px solid rgba(194, 232, 242, 0.1);">
          <h4 style="color: #82e85b; margin-top: 0;">🎯 PROFILE</h4>
          <ul style="padding-left: 20px;">
            <li>Transitioning from <strong>Electrical Engineering (FAST-NUCES)</strong> to <strong>Computer Engineering</strong></li>
            <li>Founder of <strong>WNR Production Studio</strong></li>
            <li>Passionate about open-source and hardware-software integration</li>
          </ul>
        </div>
      </div>
    </div>
  </section>

  <!-- Projects Section -->
  <section style="margin: 60px 0;">
    <h4 style="color: #82e85b; font-size: 1.5rem; margin-bottom: 20px;">🔧 KEY PROJECTS</h4>
    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 20px;">
      <div style="background: rgba(194, 232, 242, 0.05); padding: 20px; border-radius: 10px; border: 1px solid rgba(194, 232, 242, 0.1); transition: all 0.3s;" onmouseover="this.style.transform='translateY(-5px)'; this.style.boxShadow='0 10px 20px rgba(194, 232, 242, 0.1)'" onmouseout="this.style.transform='none'; this.style.boxShadow='none'">
        <h5 style="color: #c1ebf2; margin-top: 0;">🚗 Car Showroom Sales System</h5>
        <p>C++ application for inventory/customer management</p>
        <a href="https://github.com/W-N-R/Car-Showroom-Sales" target="_blank" style="color: #82e85b; text-decoration: none;">View on GitHub →</a>
      </div>
      <!--wali-->
      <div style="background: rgba(194, 232, 242, 0.05); padding: 20px; border-radius: 10px; border: 1px solid rgba(194, 232, 242, 0.1); transition: all 0.3s;" onmouseover="this.style.transform='translateY(-5px)'; this.style.boxShadow='0 10px 20px rgba(194, 232, 242, 0.1)'" onmouseout="this.style.transform='none'; this.style.boxShadow='none'">
        <h5 style="color: #c1ebf2; margin-top: 0;">💡 4x4x4 LED Cube</h5>
        <p>Arduino-powered display with multiplexed animations</p>
        <a href="https://github.com/W-N-R/LED-Cube-4x4x4" target="_blank" style="color: #82e85b; text-decoration: none;">View on GitHub →</a>
      </div>
      <div style="background: rgba(194, 232, 242, 0.05); padding: 20px; border-radius: 10px; border: 1px solid rgba(194, 232, 242, 0.1); transition: all 0.3s;" onmouseover="this.style.transform='translateY(-5px)'; this.style.boxShadow='0 10px 20px rgba(194, 232, 242, 0.1)'" onmouseout="this.style.transform='none'; this.style.boxShadow='none'">
        <h5 style="color: #c1ebf2; margin-top: 0;">🌐 Web Development</h5>
        <p>Deployed sites with 1500+ visits using HTML/CSS</p>
        <a href="https://github.com/W-N-R" target="_blank" style="color: #82e85b; text-decoration: none;">View Portfolio →</a>
      </div>
    </div>
  </section>

 
<!-- Skills Section -->
<section id="skills-section" style="margin: 60px 0;" class="skills-container">
  <h4 style="color: #82e85b; font-size: 1.5rem; margin-bottom: 20px; text-align: center;">🛠️ TECHNICAL SKILLS</h4>
  
  <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 40px; margin-top: 40px;">
    <!-- Embedded Systems - 92% -->
    <div style="text-align: center;">
      <div class="skill-circle">
        <svg viewBox="0 0 120 120">
          <circle class="circle-bg" cx="60" cy="60" r="50"></circle>
          <circle class="circle-progress" cx="60" cy="60" r="50" 
                  style="--target-offset: 25.12;"></circle> <!-- 314 * (1 - 0.92) = 25.12 -->
        </svg>
        <div style="position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%); text-align: center;">
          <span style="color: #82e85b; font-size: 1.8rem; font-weight: bold;">92%</span><br>
          <span style="color: #c1ebf2;">Embedded Systems</span>
        </div>
      </div>
    </div>
    <!-- HTML/CSS - 85% -->
    <div style="text-align: center;">
      <div class="skill-circle">
        <svg viewBox="0 0 120 120">
          <circle class="circle-bg" cx="60" cy="60" r="50"></circle>
          <circle class="circle-progress" cx="60" cy="60" r="50" 
                  style="--target-offset: 47.1;"></circle> <!-- 314 * (1 - 0.85) = 47.1 -->
        </svg>
        <div style="position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%); text-align: center;">
          <span style="color: #82e85b; font-size: 1.8rem; font-weight: bold;">85%</span><br>
          <span style="color: #c1ebf2;">HTML/CSS</span>
        </div>
      </div>
    </div>
    <!-- Git/GitHub - 99% -->
    <div style="text-align: center;">
      <div class="skill-circle">
        <svg viewBox="0 0 120 120">
          <circle class="circle-bg" cx="60" cy="60" r="50"></circle>
          <circle class="circle-progress" cx="60" cy="60" r="50" 
                  style="--target-offset: 3.14;"></circle> <!-- 314 * (1 - 0.99) = 3.14 -->
        </svg>
        <div style="position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%); text-align: center;">
          <span style="color: #82e85b; font-size: 1.8rem; font-weight: bold;">99%</span><br>
          <span style="color: #c1ebf2;">Git/GitHub</span>
        </div>
      </div>
    </div>
    <!-- 3D Animation - 80% -->
    <div style="text-align: center;">
      <div class="skill-circle">
        <svg viewBox="0 0 120 120">
          <circle class="circle-bg" cx="60" cy="60" r="50"></circle>
          <circle class="circle-progress" cx="60" cy="60" r="50" 
                  style="--target-offset: 62.8;"></circle> <!-- 314 * (1 - 0.80) = 62.8 -->
        </svg>
        <div style="position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%); text-align: center;">
          <span style="color: #82e85b; font-size: 1.8rem; font-weight: bold;">80%</span><br>
          <span style="color: #c1ebf2;">3D Animation</span>
        </div>
      </div>
    </div>
  </div>
</section>

  <!-- CTA Buttons -->
  <div style="text-align: center; margin: 50px 0;">
    <a href="https://github.com/XOST-Studio/XOST-Studio.github.io/raw/main/Muhammad%20Waleed%20Resume.pdf" 
       target="_blank"
       style="background: linear-gradient(90deg, #82e85b, #c1ebf2); 
              color: #000; 
              padding: 12px 30px; 
              border-radius: 30px; 
              text-decoration: none;
              font-weight: bold;
              font-size: 1.1rem;
              transition: all 0.3s ease;
              border: none;
              box-shadow: 0 4px 15px rgba(130, 232, 91, 0.3);
              display: inline-block;
              margin: 0 10px;"
       onmouseover="this.style.transform='scale(1.05)'; this.style.boxShadow='0 6px 20px rgba(130, 232, 91, 0.5)'" 
       onmouseout="this.style.transform='scale(1)'; this.style.boxShadow='0 4px 15px rgba(130, 232, 91, 0.3)'">
      📄 Full Resume
    </a>
    <a href="https://github.com/W-N-R" 
       target="_blank"
       style="background: transparent; 
              color: #82e85b; 
              padding: 12px 30px; 
              border-radius: 30px; 
              text-decoration: none;
              font-weight: bold;
              font-size: 1.1rem;
              transition: all 0.3s ease;
              border: 2px solid #82e85b;
              box-shadow: 0 4px 15px rgba(130, 232, 91, 0.1);
              display: inline-block;
              margin: 0 10px;"
       onmouseover="this.style.background='rgba(130, 232, 91, 0.1)'; this.style.color='#c1ebf2'; this.style.borderColor='#c1ebf2'; this.style.transform='scale(1.05)'; this.style.boxShadow='0 6px 20px rgba(194, 232, 242, 0.3)'" 
       onmouseout="this.style.background='transparent'; this.style.color='#82e85b'; this.style.borderColor='#82e85b'; this.style.transform='scale(1)'; this.style.boxShadow='0 4px 15px rgba(130, 232, 91, 0.1)'">
      💻 GitHub Portfolio
    </a>
  </div>

  <!-- Tech Stack Section -->
  <section style="margin: 60px 0;">
    <h2 style="text-align: center; font-size: 2.2rem; margin-bottom: 30px;">
      <span style="display: inline-block; background: linear-gradient(90deg, #82e85b, #c1ebf2); -webkit-background-clip: text; -webkit-text-fill-color: transparent;">
        🛠️ TECH STACK
      </span>
    </h2>
    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px;">
      <div style="background: rgba(194, 232, 242, 0.05); padding: 25px; border-radius: 10px; border-top: 3px solid #82e85b; transition: all 0.3s;" onmouseover="this.style.transform='translateY(-5px)'; this.style.boxShadow='0 10px 25px rgba(130, 232, 91, 0.1)'" onmouseout="this.style.transform='none'; this.style.boxShadow='none'">
        <h4 style="color: #c1ebf2; margin-top: 0; font-size: 1.3rem;">🔷 Frontend</h4>
        <p style="margin-bottom: 0;">HTML5 / CSS3 / JavaScript</p>
      </div>
      <div style="background: rgba(194, 232, 242, 0.05); padding: 25px; border-radius: 10px; border-top: 3px solid #c1ebf2; transition: all 0.3s;" onmouseover="this.style.transform='translateY(-5px)'; this.style.boxShadow='0 10px 25px rgba(194, 232, 242, 0.1)'" onmouseout="this.style.transform='none'; this.style.boxShadow='none'">
        <h4 style="color: #c1ebf2; margin-top: 0; font-size: 1.3rem;">⚛️ Animations</h4>
        <p style="margin-bottom: 0;">GSAP, CSS3, Lottie</p>
      </div>
      <div style="background: rgba(194, 232, 242, 0.05); padding: 25px; border-radius: 10px; border-top: 3px solid #82e85b; transition: all 0.3s;" onmouseover="this.style.transform='translateY(-5px)'; this.style.boxShadow='0 10px 25px rgba(130, 232, 91, 0.1)'" onmouseout="this.style.transform='none'; this.style.boxShadow='none'">
        <h4 style="color: #c1ebf2; margin-top: 0; font-size: 1.3rem;">🌀 Layout</h4>
        <p style="margin-bottom: 0;">Responsive, mobile-first</p>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer style="text-align: center; margin-top: 80px; padding: 30px 0; color: #c1ebf2; font-size: 0.9em; border-top: 1px solid rgba(194, 232, 242, 0.2); position: relative;">
    <div style="position: absolute; top: 0; left: 50%; transform: translateX(-50%); width: 30%; height: 1px; background: linear-gradient(90deg, transparent, #82e85b, #c1ebf2, transparent);"></div>
    <p style="margin: 10px 0;">© 2025 XOST Studio | Building the next-gen digital experiences</p>
    <p style="margin: 10px 0;">Project maintained by <a href="https://github.com/W-N-R" style="color: #82e85b; text-decoration: none; transition: all 0.3s;" onmouseover="this.style.textShadow='0 0 8px #82e85b'" onmouseout="this.style.textShadow='none'">WNR</a></p>
    <div style="display: flex; justify-content: center; gap: 15px; margin-top: 20px;">
      <a href="#" style="color: #c1ebf2; text-decoration: none; transition: all 0.3s;" onmouseover="this.style.color='#82e85b'; this.style.transform='scale(1.2)'" onmouseout="this.style.color='#c1ebf2'; this.style.transform='scale(1)'">Twitter</a>
      <a href="#" style="color: #c1ebf2; text-decoration: none; transition: all 0.3s;" onmouseover="this.style.color='#82e85b'; this.style.transform='scale(1.2)'" onmouseout="this.style.color='#c1ebf2'; this.style.transform='scale(1)'">LinkedIn</a>
      <a href="#" style="color: #c1ebf2; text-decoration: none; transition: all 0.3s;" onmouseover="this.style.color='#82e85b'; this.style.transform='scale(1.2)'" onmouseout="this.style.color='#c1ebf2'; this.style.transform='scale(1)'">Instagram</a>
    </div>
  </footer>
</div>
