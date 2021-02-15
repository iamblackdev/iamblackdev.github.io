<template>
  <div id="home" class="home" >
    <div v-if="active" class="mobile_top fixed-top w-100"></div>
    <div class="container">
      <div   class="row">
        <div class="col-lg-5 intro">

          <div class="intro-card">
            <div class="heading">
              <h1>Hello, I’m Wahab Habib.</h1>
            </div>
            <div class="bio-paragraph">
              <p>I’m a Software Engineer. I'm frontend developer and i'm based in Nigeria.</p>
              <p>
                I'm usually somewhere on the internet. You can find me oversharing on
                <a target="_blank" href="https://twitter.com/black_dev_">twitter</a>, exploring
                <a target="_blank" href="https://www.facebook.com/habib.wahab.16">facebook</a> contents, posting exciting projects on
                <a target="_blank" href="https://github.com/iamblackdev">github</a>, or occasionally looking for new stuff to learn.
              </p>
            </div>

          <div id="list-example" class="nav ">
            <ul>
              <li class="">
                 <a class="list-group-item" href="#home">
                    <span class="mr-2">01</span>
                    <span class="nav-line mr-2 d-inline-block"></span>
                    <span>Projects</span>
                  </a>
              </li>
              <li>
                 <a class="list-group-item" href="#about">
                    <span class="mr-2">02</span>
                    <span class="nav-line mr-2 d-inline-block"></span>
                    <span>About</span>
                  </a>
              </li>
              <li >
                 <a class="list-group-item" href="#contacts">
                    <span class="mr-2">03</span>
                    <span class="nav-line mr-2 d-inline-block"></span>
                    <span>Contact</span>
                  </a>
              </li>
            </ul>
          </div>

          <div class="socials mt-4 mb-5">
            <ul>

              <li class="mx-3">
                <a href="https://twitter.com/black_dev_" rel="noopener" target="_blank" class="flex items-center">
                  <svg xmlns="http://www.w3.org/2000/svg" class="mr-2" viewBox="0 0 24 24" style="fill:white" aria-hidden="true" width="16" height="16" ><title>Twitter icon</title><path d="M24 4.557a9.83 9.83 0 01-2.828.775 4.932 4.932 0 002.165-2.724 9.864 9.864 0 01-3.127 1.195 4.916 4.916 0 00-3.594-1.555c-3.179 0-5.515 2.966-4.797 6.045A13.978 13.978 0 011.671 3.149a4.93 4.93 0 001.523 6.574 4.903 4.903 0 01-2.229-.616c-.054 2.281 1.581 4.415 3.949 4.89a4.935 4.935 0 01-2.224.084 4.928 4.928 0 004.6 3.419A9.9 9.9 0 010 19.54a13.94 13.94 0 007.548 2.212c9.142 0 14.307-7.721 13.995-14.646A10.025 10.025 0 0024 4.557z"></path></svg>
                  <span class="mt-px">Twitter</span>
                  <span class="w-16 p-2 ml-8">
                  <svg xmlns="http://www.w3.org/2000/svg" fill="none" width="16" height="16" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 12 12" aria-hidden="true" class="flex-none stroke-current"><title>External link icon</title><path d="M10.976 1.193A.314.314 0 0010.687 1H6.312a.313.313 0 000 .625h3.62L5.467 6.091a.313.313 0 00.443.442l4.466-4.466v3.62a.313.313 0 00.625 0V1.313a.328.328 0 00-.024-.119z"></path><path d="M3.5 1v.625H2.25a.625.625 0 00-.625.625v7.5c0 .345.28.625.625.625h7.5c.345 0 .625-.28.625-.625V8.5H11v1.875c0 .345-.28.625-.625.625h-8.75A.625.625 0 011 10.375v-8.75C1 1.28 1.28 1 1.625 1H3.5z"></path></svg>
                  </span>
                </a>
              </li>

              <li class="mx-3">
                <a href="https://github.com/iamblackdev" rel="noopener" target="_blank" class="flex items-center">
                  <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" class="mr-3" style="fill:white" width="16" height="16" aria-hidden="true"><title>GitHub icon</title><path d="M12 .297c-6.63 0-12 5.373-12 12 0 5.303 3.438 9.8 8.205 11.385.6.113.82-.258.82-.577 0-.285-.01-1.04-.015-2.04-3.338.724-4.042-1.61-4.042-1.61C4.422 18.07 3.633 17.7 3.633 17.7c-1.087-.744.084-.729.084-.729 1.205.084 1.838 1.236 1.838 1.236 1.07 1.835 2.809 1.305 3.495.998.108-.776.417-1.305.76-1.605-2.665-.3-5.466-1.332-5.466-5.93 0-1.31.465-2.38 1.235-3.22-.135-.303-.54-1.523.105-3.176 0 0 1.005-.322 3.3 1.23.96-.267 1.98-.399 3-.405 1.02.006 2.04.138 3 .405 2.28-1.552 3.285-1.23 3.285-1.23.645 1.653.24 2.873.12 3.176.765.84 1.23 1.91 1.23 3.22 0 4.61-2.805 5.625-5.475 5.92.42.36.81 1.096.81 2.22 0 1.606-.015 2.896-.015 3.286 0 .315.21.69.825.57C20.565 22.092 24 17.592 24 12.297c0-6.627-5.373-12-12-12"></path></svg>
                  <span class="mt-px">GitHub</span>
                  <span class="w-16 p-2 ml-8">
                  <svg xmlns="http://www.w3.org/2000/svg" fill="none" width="16" height="16" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 12 12" aria-hidden="true" class="flex-none stroke-current"><title>External link icon</title><path d="M10.976 1.193A.314.314 0 0010.687 1H6.312a.313.313 0 000 .625h3.62L5.467 6.091a.313.313 0 00.443.442l4.466-4.466v3.62a.313.313 0 00.625 0V1.313a.328.328 0 00-.024-.119z"></path><path d="M3.5 1v.625H2.25a.625.625 0 00-.625.625v7.5c0 .345.28.625.625.625h7.5c.345 0 .625-.28.625-.625V8.5H11v1.875c0 .345-.28.625-.625.625h-8.75A.625.625 0 011 10.375v-8.75C1 1.28 1.28 1 1.625 1H3.5z"></path></svg>
                  </span>
                </a>
              </li>

            </ul>
          </div>


          </div>
        </div>

        <!-- ASIDE -->
        <div class="col-lg-6 ml-auto">
          
          <div data-spy="scroll" data-target="#list-example" data-offset="0">


            <div id="projects">
              <h2 class="section-header js-scroll-trigger sticky-top">projects</h2>
              
              <a v-for="work in works" :key="work" target="_blank" :href="work.link">
                <div @mouseenter="projectEnter" @mouseleave="projectLeave" class="project-card">
                <p class="card-heading">
                  {{work.techUsed}}
                </p>
                <h3 class="project-title">
                  {{work.name}}
                </h3>
                <p class="project-description">
                 {{work.description}}
                </p>

                </div>
              </a>
              
              
            </div>

            <div id="about"></div>
            <div class=" about">

              
                <h2 class="w-100 section-header sticky-top">About</h2> 
              
                <div class="about-card ">

                  <p>
                   I'm a Frontend web developer based in Nigeria, working with different web technologies to build projects i find intresting and having direct impact on people, while following best practices applicable. I'm capable of learning and working with new technologies swiftly.
                  </p>
                  <p>
                     Most of my time is spent on learning new technologies in the web to build awesome stuffs.
                  </p>
                  <p>
                    Outside being a techy, I hangout with few friends and try not to be an introvert in reality while being social on social media, 😊.     
                  </p>


                </div>             

            </div>

            <div id="contacts"></div>
            <div class="contact">
              <h2 class="section-header sticky-top">Contact</h2>
              <div class="row">
                <div v-if="loader" class="col-11 mx-auto d-flex justify-content-center align-items-center position-absolute w-100 loader " style="">
                  <div class="sk-chase">
                    <div class="sk-chase-dot"></div>
                    <div class="sk-chase-dot"></div>
                    <div class="sk-chase-dot"></div>
                    <div class="sk-chase-dot"></div>
                    <div class="sk-chase-dot"></div>
                    <div class="sk-chase-dot"></div>
                  </div>
                </div>
                <div class="col-11 mx-auto mt-4 contact-card">
                  <div class="h4 text-white text-center mb-4 d-md-none">Send me an email</div>
                  <div class="alert alert-success display_alert" role="alert" style="display: none;">
                    <small>Email sent. I'll get back to you shortly.</small>
                  </div>

                  <form id="contact_form" method="POST" v-on:submit.prevent="handleFormSubmit">
                    <div class="form-group">
                      <input
                        type="text"
                        class="form-control"
                        name="full_name"
                        placeholder="Full name"
                        required
                      />
                    </div>
                    <div class="form-group mt-5">
                      <input
                        type="email"
                        class="form-control"
                        name="user_email"
                        placeholder="Email address"
                        required
                      />
                    </div>
                    <div class="form-group mt-5">
                      <input
                        type="tel"
                        class="form-control"
                        name="phone"
                        placeholder="Phone"
                        required
                      />
                    </div>
                    <div class="form-group mt-5">
                      <textarea
                        class="form-control"
                        rows="4"
                        name="message"
                        placeholder="Message"
                        required
                      ></textarea>
                    </div>
                    <button type="submit"  class="btn btn-default btn_send w-100 mt-2 text-white">Send</button>
                  </form>
                  
                </div>
              </div>

            </div>

          </div>
          
        </div>

      </div>
    </div>
  </div>
</template>

<script>
import Json from '../../public/works.json'
import emailjs from "emailjs-com";
export default {
  name: 'home',
  data(){
    return{
      active: false,
      loader: false,
      works: Json
    }
  },
  created () {
    window.addEventListener('scroll', this.handleScroll);
  },
  destroyed () {
    window.removeEventListener('scroll', this.handleScroll);
  },
 methods:{
   handleScroll () {
      
      let  rect = document.querySelector('#projects').getBoundingClientRect();
      if (rect.top < -11){
        this.active = true
      }else{
        this.active = false
      } 
    },
   projectEnter(e){
    e.target.parentElement.querySelectorAll('.project-card').forEach(card => {
      card.style.opacity = '0.5'
    });
    e.target.style.opacity = '1'     
     
   },
   projectLeave(e){
      e.target.parentElement.querySelectorAll('.project-card').forEach(card => {
      card.style.opacity = '1'
    });
   },
   handleFormSubmit: function(e){
      this.loader = true
      e.preventDefault();
      emailjs.sendForm("gmail", "template_I9TVCcd4", e.target, "user_malZEJsd7ijKbv4lMYiRA")
        .then(
          (result) => {
            if (result){
              document.getElementById("contact_form").reset();
            document.querySelector(".display_alert").style.display = "block";
            this.loader = false 
            setTimeout(() => {
              document.querySelector(".display_alert").style.display = "none";
            }, 2500);
            }
            
          },
          (error) => {
            alert("An error occured, Please try again", error.text);
          }
        );
    },
 }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
/* utilities */
.card-heading{
  font-size: 10px;
  font-weight: 700;
  letter-spacing: 3px;
  text-transform: uppercase;
  color: white;
}
.section-header{
  display: none;
}
.mobile_top{
  display: none;
}
.container{
  padding-top: 80px;

}
.intro{
  position: fixed;
}
.intro-card{
  width: 450px;
}
.heading h1{
  font-size: 64px;
  font-weight: bold;
}
.bio-paragraph{
  margin-top: 32px;
  color: rgb(148, 148, 149);
  line-height: 28px;
}
.bio-paragraph a:hover{
  color: inherit;
}
.nav{
  margin-top: 52px;
}
.nav ul {
  list-style: none;
}
.nav ul li{
  margin: 26px 0px;
}
.nav ul li a{
  letter-spacing: 3px;
  font-size: 10px;
  text-decoration: none;
  color: rgb(148, 148, 149);
  text-transform: uppercase;
}
.nav .nav-line{
  width: 24px;
  border-bottom: 1px solid rgb(148, 148, 149);
  transition: all .3s ease;
}
.nav li:hover a, .nav li a.active{
  color: white;
}
.nav li:hover .nav-line, .nav a.active .nav-line{
  border-color: white;
  width: 48px;
}
.list-group-item {
    position: relative;
    display: block;
    padding: 0;
    background-color: transparent;
    border:0;
}
.socials ul{
 list-style: none;
}
.socials ul {
  display: flex;
  flex-wrap: wrap;
  flex-direction: row;
}
.socials ul li a:hover {
  color: white;
  text-decoration: none;
}

/*  */
#projects a:hover{
  text-decoration: none;
  color: inherit;
}
.project-card{
  padding: 40px;
   --bg-opacity: 1;
    background-color: #202022;
    background-color: rgba(32,32,34,var(--bg-opacity));
    transition: all .3s ease;
    margin-bottom: 10px;
}
.project-card:hover{
  transform: scale(1.15);
}

.project-title{
  margin-top: 20px;
  line-height: 1.25px;
  font-size: 24px;
  font-weight: 600;
}

.project-description{
  margin-top: 20px;
  font-size: 14px;
  color: rgb(148, 148, 149);
}
.project-rating svg{
  color: rgb(148, 148, 149);
}
.rating-count{
  color: rgb(148, 148, 149);
  font-size: 10px;
  font-weight: 600;
  letter-spacing: 2px;
}
/*  */
.about{
  margin-top: 90px;
}
.about-card{
  padding: 40px;
   --bg-opacity: 1;
    background-color: #202022;
    background-color: rgba(32,32,34,var(--bg-opacity));
    transition: all .3s ease;
    margin-bottom: 10px;
    margin: 5px;
    font-size: 18px;
}


/*  */
.contact{
  margin-top: 100px;
}
.contact a{
  text-decoration: none;
  
}
.contact-card {
    padding: 40px;
   --bg-opacity: 1;
    background-color: #202022;
    background-color: rgba(32,32,34,var(--bg-opacity));
    transition: all .3s ease;
    margin-bottom: 10px;
    margin: 5px;
    font-size: 18px;
}

.form-control {
  background-color: #202022;
  border-left: none;
  border-right: none;
  border-top: none;
  border-radius: 0px !important;
  font-size: 16px;
  box-shadow: none;
}

/*  */
.loader{
  margin-top: 23px;
  height: 510px;
  z-index:10; 
  background-color:#202022; 
  opacity:0.5;
  left: 25px;

}
.sk-chase {
  width: 40px;
  height: 40px;
  position: relative;
  animation: sk-chase 2.5s infinite linear both;
}

.sk-chase-dot {
  width: 100%;
  height: 100%;
  position: absolute;
  left: 0;
  top: 0; 
  animation: sk-chase-dot 2.0s infinite ease-in-out both; 
}

.sk-chase-dot:before {
  content: '';
  display: block;
  width: 25%;
  height: 25%;
  background-color: #fff;
  border-radius: 100%;
  animation: sk-chase-dot-before 2.0s infinite ease-in-out both; 
}

.sk-chase-dot:nth-child(1) { animation-delay: -1.1s; }
.sk-chase-dot:nth-child(2) { animation-delay: -1.0s; }
.sk-chase-dot:nth-child(3) { animation-delay: -0.9s; }
.sk-chase-dot:nth-child(4) { animation-delay: -0.8s; }
.sk-chase-dot:nth-child(5) { animation-delay: -0.7s; }
.sk-chase-dot:nth-child(6) { animation-delay: -0.6s; }
.sk-chase-dot:nth-child(1):before { animation-delay: -1.1s; }
.sk-chase-dot:nth-child(2):before { animation-delay: -1.0s; }
.sk-chase-dot:nth-child(3):before { animation-delay: -0.9s; }
.sk-chase-dot:nth-child(4):before { animation-delay: -0.8s; }
.sk-chase-dot:nth-child(5):before { animation-delay: -0.7s; }
.sk-chase-dot:nth-child(6):before { animation-delay: -0.6s; }

@keyframes sk-chase {
  100% { transform: rotate(360deg); } 
}

@keyframes sk-chase-dot {
  80%, 100% { transform: rotate(360deg); } 
}

@keyframes sk-chase-dot-before {
  50% {
    transform: scale(0.4); 
  } 100%, 0% {
    transform: scale(1.0); 
  } 
}

@media (min-width: 1200px) { 
  .container{
      max-width: 1250px !important;
  }
 }

@media (max-width: 1199.98px) { 
  .loader{
  left: 22px;
  }
 }
@media (max-width: 991.98px) { 
  .container{
    padding-top: 20px;
  }
  .intro{
    position: static;
  }
  .heading h1{
    font-size: 48px;
  }
  .intro-card{
    width: 100%;
  }
  .nav{
    display: none;
  }
  .section-header{
    padding: 24px 0px;
    display: block;
    font-size: 12px;
    text-transform: uppercase;
    letter-spacing: 3px;
    z-index: 999999;
  }
  .project-card:hover{
    transform: scale(1);
  }
  .loader{
    left: 29px;
  }
  .contact{
    margin-bottom: 20px;
  }
  .mobile_top{
    display: inline-block;
    height: 60px;
    background-color: #202022;
  }
 }

@media (max-width: 767.98px) { 
  .bio-paragraph{
    font-size: 18px;
  }
  .project-title{
    line-height: 30px;
  }
  .contact{
  margin-top: 20px;
  margin-bottom: 10px;
  }
  .loader{
    left: 15px;
  }
}
@media (max-width: 575.98px) {  }

</style>
