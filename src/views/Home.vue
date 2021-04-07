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
              <p>I’m a Software Engineer, particularly a frontend developer based in Nigeria.</p>
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
                 <a class="list-group-item active" href="#home">
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
              <li>
                 <a class="list-group-item" href="#contacts">
                    <span class="mr-2">03</span>
                    <span class="nav-line mr-2 d-inline-block"></span>
                    <span>Contact</span>
                  </a>
              </li>
            </ul>
          </div>

          <div class="socials mt-5 mt-lg-0 mb-5">
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


            <Projects />

            <div id="about"></div>
            <About />

            <div id="contacts"></div>
            <Contact />
           

          </div>
          
        </div>

      </div>
    </div>
  </div>
</template>

<script>
import Projects from '../components/projects.vue'
import About from '../components/about.vue'
import Contact from '../components/contact.vue'

export default {
  components:{ 
    Projects,
    About,
    Contact
  },
  data() {
    return {
      active: false
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
   
 }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
/* utilities */
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

/* NAV */
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

.list-group-item {
    position: relative;
    display: block;
    padding: 0;
    background-color: transparent;
    border:0;
}
.nav li:hover a, .nav li .list-group-item.active{
  color: white;
}
.nav li:hover .nav-line, .nav .list-group-item.active .nav-line{
  border-color: white;
  width: 48px;
}
.list-group-item.active{
  background-color: transparent;
}

/* SOCIALS */
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



@media (min-width: 1200px) { 
  .container{
      max-width: 1250px !important;
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
  
}

</style>
