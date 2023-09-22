<template>
    <body>
    <div id="header">
<div class="container">
<nav>
    <img src="../assets/images/logo.png" class="logo">
    <ul id="sidemenu">
      <li><a href="#header">Home</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#services">Services</a></li>
      <li><a href="#portfolio">Portfolio</a></li>
      <li><a href="#contact">Contact</a></li>
      <i class="fa-solid fa-xmark" @click="closemenu()"></i>
    </ul>
    <i class="fa-solid fa-bars" @click="openmenu()"></i>
</nav>
<div class="home-text">
    <h3>Fullstack Web Developer</h3>
    <h1>Hi, I'm <span>Moemen</span><br>A Software Architecture Engineer</h1>
</div>


</div>
    </div>
    <!-- ----------about----------- -->
<div id="about">
    <div class="container">
        <div class="row">
            <div class="about-col-1">
                <img src="../assets/images/user.png">
            </div>
            <div class="about-col-2">
                <h1 class="subtitle">About Me</h1>
                <p>I'm a young software architecture candidate with a passion for
                 computer science, eager to learn new skills and thirsty for knowledge. I'm a person with a
                great communication skills always looking for new experiences and new challenges.</p>
                    <div class="tabtitle">
                        <p class="tab-links active-link" @click="opentab('skills')">Skills</p>
                        <p class="tab-links" @click="opentab('experience')">Experience</p>
                        <p class="tab-links" @click="opentab('education')">Education</p>
                    </div>
                    <div class="tab-contents active-tab" id="skills">
                        <ul>
                            <li><span>UI/UX</span><br>Designing Web/App interfaces</li>
                            <li><span>Web Development</span><br>Web App Development</li>
                            <li><span>Devops</span><br>Devops devops devops</li>
                        </ul>
                    </div>
                    <div class="tab-contents" id="experience">
                        <ul>
                            <li><span>UI/UX</span><br>Designing Web/App</li>
                            <li><span>Web Development</span><br>Web App Development</li>
                            <li><span>Devops</span><br>Devops devops devops</li>
                        </ul>
                    </div>
                    <div class="tab-contents" id="education">
                        <ul>
                            <li><span>UI/UX</span><br>Designing Web/App interfaces</li>
                            <li><span>Web Development</span><br>Web App Development</li>
                            <li><span>Devops</span><br>Devops </li>
                        </ul>
                    </div>
            </div>
        </div>
    </div>
</div>

<!-- ----------------services---------------- -->

<div id="services">
    <div class="container">
        <h1 class="subtitle">My Services</h1>
        <div class="services-list">
            <div>
                <i class="fa-solid fa-code"></i>
                <h2>Web Design</h2>
                <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Velit, alias soluta accusamus nobis, culpa suscipit illo quia, sed cumque dolore pariatur 
                    aspernatur quibusdam maiores libero ex. Sit corporis hic aliquid?</p>
                    <a href="#">Learn more</a>
            </div>
            <div>
                <i class="fa-solid fa-crop"></i>
                <h2>UI/UX Design</h2>
                <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Velit, alias soluta accusamus nobis, culpa suscipit illo quia, sed cumque dolore pariatur 
                    aspernatur quibusdam maiores libero ex. Sit corporis hic aliquid?</p>
                    <a href="#">Learn more</a>
            </div>
            <div>
                <i class="fa-brands fa-app-store"></i>
                <h2>App Design</h2>
                <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Velit, alias soluta accusamus nobis, culpa suscipit illo quia, sed cumque dolore pariatur 
                    aspernatur quibusdam maiores libero ex. Sit corporis hic aliquid?</p>
                    <a href="#">Learn more</a>
            </div>
        </div>
    </div>
</div>

<!-- ----------------portfolio------------------- -->

<div id="portfolio">
    <div class="container">
        <h1 class="subtitle">My Work</h1>
        <div class="work-list">
            <div class="work">
                <img src="../assets/images/work-1.png">
                <div class="layer">
                    <h3>Medical Office App</h3>
                    <p>
                        Design and development of a medical office management application.  
                    </p>
                    <a href="#"><i class="fa-solid fa-arrow-up-right-from-square"></i></a>
                </div>
            </div>
            <div class="work">
                <img src="../assets/images/work-2.png">
                <div class="layer">
                    <h3>Gaming E-Commerce Web Site</h3>
                    <p>
                        Development of an E - commerce website dedicated to gaming products and the
organization of tournaments and events.                    </p>
                    <a href="#"><i class="fa-solid fa-arrow-up-right-from-square"></i></a>
                </div>
            </div>
            <div class="work">
                <img src="../assets/images/work-3.png">
                <div class="layer">
                    <h3>Agriculture E-Commerce Web Site</h3>
                    <p>
                        Development of an E-commerce website for the sale of agricultural products.

                    </p>
                    <a href="#"><i class="fa-solid fa-arrow-up-right-from-square"></i></a>
                </div>
            </div>
        </div>
        <a href="#" class="btn">See more</a>
    </div>
</div>

<!-- ---------------contact------------------ -->
<div id="contact">
    <div class="container">
        <div class="row">
            <div class="contact-left">
                <h1 class="subtitle">Contact Me</h1>
                <p><i class="fa-solid fa-paper-plane"></i>Contact@example.com</p>
                <p><i class="fa-solid fa-square-phone"></i>55238213</p>
                <div class="social-icons">
                    <a href="https://facebook.com/"><i class="fa-brands fa-facebook"></i></a>
                    <a href="#"><i class="fa-brands fa-instagram"></i></a>
                    <a href="#"><i class="fa-brands fa-linkedin"></i></a>
                    <a href="#"><i class="fa-brands fa-github"></i></a>
                </div>
                <a href="../assets/mycv.pdf" download class="btn btn2">Download CV</a>
            </div>
            <div class="contact-right">
                <form action="">
                    <input type="text" name="Name" placeholder="Your Name" required>
                    <input type="email" name="Email" placeholder="Your Email" required>
                    <textarea name="Message" rows="6" placeholder="YourMessage"></textarea>
                    <button type="submit" class="btn btn2">Submit</button>
                </form>
            </div>
        </div>
    </div>
    <div class="copyright">
        <p>&copy; {{ currentYear }} Abdelmoemen Trabelsi. <i class="fa-solid fa-heart"></i> All rights reserved.</p>
    </div>
</div>
</body>
</template>

<script>
export default {
  name: "HomePage",
  data() {
    return {
      currentYear: new Date().getFullYear(),
    };
  },
  methods: {
opentab(tabname){

    const tablinks = document.getElementsByClassName("tab-links");
    const tabcontents = document.getElementsByClassName("tab-contents");

    for( const tablink of tablinks){
        tablink.classList.remove("active-link");
    }
    for(const tabcontent of tabcontents){
        tabcontent.classList.remove("active-tab");
    }
    event.currentTarget.classList.add("active-link");
    document.getElementById(tabname).classList.add("active-tab");
},
openmenu(){
    const sidemeu= document.getElementById("sidemenu");
    sidemeu.style.right = "0";
},
closemenu(){
    const sidemeu= document.getElementById("sidemenu");
    sidemeu.style.right = "-200px";
}
  }
};





</script>
