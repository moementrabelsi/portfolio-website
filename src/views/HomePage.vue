<template>
    <body>
    <div class="header">
<div class="container">
<nav>
    <img src="../assets/images/logo.png" class="logo">
    <ul>
      <li><router-link to="/" exact class="nav-link active">Home</router-link></li>
      <li><router-link to="/about" class="nav-link">About</router-link></li>
      <li><router-link to="/services" class="nav-link">Services</router-link></li>
      <li><router-link to="/portfolio" class="nav-link">Portfolio</router-link></li>
      <li><router-link to="/contact" class="nav-link">Contact</router-link></li>
    </ul>
</nav>
<div class="home-text">
    <h3>Fullstack Web Developer</h3>
    <h1>Hi, I'm <span>Moemen</span><br>A Software Architecture</h1>
    <P>Lorem ipsum dolor sit amet consectetur adipisicing elit. <br>Perferendis provident corrupti nihil aliquid possimus, <br>culpa atque rerum inventore consequuntur. <br>Repellat tempore mollitia iure quam, quisquam <br>animi magni iusto vero perspiciatis.</P>
</div>


</div>
    </div>
    <!-- ----------about----------- -->
<div class="about">
    <div class="container">
        <div class="row">
            <div class="about-col-1">
                <img src="../assets/images/user.png">
            </div>
            <div class="about-col-2">
                <h1 class="subtitle">About Me</h1>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. 
                    Quasi, maxime debitis incidunt unde illo voluptatum exercitationem ullam esse, 
                    iusto libero quis totam perferendis, ducimus nulla dolores alias.</p>
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
</body>
</template>

<script>
export default {
  name: "HomePage",
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
}
  }
};


</script>
