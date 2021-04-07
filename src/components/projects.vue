<template>
    <div>
        <div id="projects">
              <h2 class="section-header js-scroll-trigger sticky-top">Projects</h2>
              
              <a v-for="work in works" :key="work.name" target="_blank" :href="work.link">
                <div @mouseenter="projectEnter(work)" @mouseleave="projectLeave(work)" class="project-card" :class="{projectCardHoverEffect: work.projectActive}">
                <p class="tech-used">
                  {{work.techUsed}}
                </p>
                <h3 class="project-title">
                  {{work.name}}
                </h3>
                <p class="project-description">
                 {{work.description}}
                </p>
                <a target="_blank" :href="work.github">
                  <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" class="mr-3" style="fill:white" width="16" height="16" aria-hidden="true"><title>GitHub icon</title><path d="M12 .297c-6.63 0-12 5.373-12 12 0 5.303 3.438 9.8 8.205 11.385.6.113.82-.258.82-.577 0-.285-.01-1.04-.015-2.04-3.338.724-4.042-1.61-4.042-1.61C4.422 18.07 3.633 17.7 3.633 17.7c-1.087-.744.084-.729.084-.729 1.205.084 1.838 1.236 1.838 1.236 1.07 1.835 2.809 1.305 3.495.998.108-.776.417-1.305.76-1.605-2.665-.3-5.466-1.332-5.466-5.93 0-1.31.465-2.38 1.235-3.22-.135-.303-.54-1.523.105-3.176 0 0 1.005-.322 3.3 1.23.96-.267 1.98-.399 3-.405 1.02.006 2.04.138 3 .405 2.28-1.552 3.285-1.23 3.285-1.23.645 1.653.24 2.873.12 3.176.765.84 1.23 1.91 1.23 3.22 0 4.61-2.805 5.625-5.475 5.92.42.36.81 1.096.81 2.22 0 1.606-.015 2.896-.015 3.286 0 .315.21.69.825.57C20.565 22.092 24 17.592 24 12.297c0-6.627-5.373-12-12-12"></path></svg>
                </a>
                </div>
              </a>      
        </div>
    </div>  
</template>

<script>
import Json from '../../public/works.json'


export default {
    data() {
        return {
            works: Json
        }
    },
    methods:{
        projectEnter(work){
            this.works.forEach(e => {
                e.projectActive = true
            });
            work.projectActive = false
            
        },
        projectLeave(){
            this.works.forEach(e => {
                e.projectActive = false
            });
            
        },
    }
}
</script>

<style>

#projects a:hover{
  text-decoration: none;
  color: inherit;
}
.project-card{
    padding: 40px;
    background-color: rgba(32,32,34,var(--bg-opacity));
    transition: all .3s ease;
    margin-bottom: 10px;
}
.project-card:hover{
  transform: scale(1.15);
}
.tech-used{
  font-size: 10px;
  font-weight: 700;
  letter-spacing: 3px;
  text-transform: uppercase;
  color: white;
}
.projectCardHoverEffect{
    opacity: 0.5;
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
@media (max-width:991.98px) {
  .project-card:hover{
    transform: scale(1);
  }
}
@media (max-width: 767.98px) { 
  .project-title{
    line-height: 30px;
  }
  
}

</style>