<template>
  <div id="home" class="home" >
    <div v-if="active" class="mobile_top fixed-top w-100"></div>
    <div class="container">
      <div   class="row">
        <div class="col-lg-5 intro">

          <div class="intro-card">
            <div class="heading">
              <h1>Hello, I’m Sarah Dayan.</h1>
            </div>
            <div class="bio-paragraph">
              <p>I’m a Staff Software Engineer currently working as Tech Lead of the Doc Squad at Algolia. I mostly do front-end development, and I’m a Vue.js and CSS nerd. I can't shut up about test-driven development and utility-first CSS. I also share what I learn on my blog frontstuff.io, or at meetups and conferences.</p>
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
                 <a class="list-group-item" href="#talks">
                    <span class="mr-2">02</span>
                    <span class="nav-line mr-2 d-inline-block"></span>
                    <span>Talks</span>
                  </a>
              </li>
              <li >
                 <a class="list-group-item" href="#interviews">
                    <span class="mr-2">03</span>
                    <span class="nav-line mr-2 d-inline-block"></span>
                    <span>interviews</span>
                  </a>
              </li>
            </ul>
          </div>

          <div class="socials mt-4 mb-5">
            <ul>

              <li class="mx-3">
                <a href="https://twitter.com/frontstuff_io" rel="noopener" target="_blank" class="flex items-center">
                  <svg xmlns="http://www.w3.org/2000/svg" class="mr-2" viewBox="0 0 24 24" style="fill:white" aria-hidden="true" width="16" height="16" ><title>Twitter icon</title><path d="M24 4.557a9.83 9.83 0 01-2.828.775 4.932 4.932 0 002.165-2.724 9.864 9.864 0 01-3.127 1.195 4.916 4.916 0 00-3.594-1.555c-3.179 0-5.515 2.966-4.797 6.045A13.978 13.978 0 011.671 3.149a4.93 4.93 0 001.523 6.574 4.903 4.903 0 01-2.229-.616c-.054 2.281 1.581 4.415 3.949 4.89a4.935 4.935 0 01-2.224.084 4.928 4.928 0 004.6 3.419A9.9 9.9 0 010 19.54a13.94 13.94 0 007.548 2.212c9.142 0 14.307-7.721 13.995-14.646A10.025 10.025 0 0024 4.557z"></path></svg>
                  <span class="mt-px">Twitter</span>
                  <span class="w-16 p-2 ml-8">
                  <svg xmlns="http://www.w3.org/2000/svg" fill="none" width="16" height="16" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 12 12" aria-hidden="true" class="flex-none stroke-current"><title>External link icon</title><path d="M10.976 1.193A.314.314 0 0010.687 1H6.312a.313.313 0 000 .625h3.62L5.467 6.091a.313.313 0 00.443.442l4.466-4.466v3.62a.313.313 0 00.625 0V1.313a.328.328 0 00-.024-.119z"></path><path d="M3.5 1v.625H2.25a.625.625 0 00-.625.625v7.5c0 .345.28.625.625.625h7.5c.345 0 .625-.28.625-.625V8.5H11v1.875c0 .345-.28.625-.625.625h-8.75A.625.625 0 011 10.375v-8.75C1 1.28 1.28 1 1.625 1H3.5z"></path></svg>
                  </span>
                </a>
              </li>

              <li class="mx-3">
                <a href="https://github.com/sarahdayan/" rel="noopener" target="_blank" class="flex items-center">
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
              <div @mouseenter="projectEnter" @mouseleave="projectLeave" class="project-card">
                <p class="card-heading">
                  javascript
                </p>
                <h3 class="project-title">
                  Dinero.js
                </h3>
                <p class="project-description">
                  An immutable JavaScript library to create, calculate and format money.
                </p>
                <div class="project-rating">
                  <span>
                    <svg width="1em" height="1em" viewBox="0 0 16 16" class="bi bi-star-fill" fill="currentColor" xmlns="http://www.w3.org/2000/svg">
                    <path d="M3.612 15.443c-.386.198-.824-.149-.746-.592l.83-4.73L.173 6.765c-.329-.314-.158-.888.283-.95l4.898-.696L7.538.792c.197-.39.73-.39.927 0l2.184 4.327 4.898.696c.441.062.612.636.283.95l-3.523 3.356.83 4.73c.078.443-.36.79-.746.592L8 13.187l-4.389 2.256z"/>
                  </svg>
                  </span>
                  <span class="ml-2 rating-count">
                    3,840
                  </span>
                </div>

              </div>
              <div @mouseenter="projectEnter" @mouseleave="projectLeave" class="project-card">
                <p class="card-heading">
                  javascript
                </p>
                <h3 class="project-title">
                  Dinero.js
                </h3>
                <p class="project-description">
                  An immutable JavaScript library to create, calculate and format money.
                </p>
                <div class="project-rating">
                  <span>
                    <svg width="1em" height="1em" viewBox="0 0 16 16" class="bi bi-star-fill" fill="currentColor" xmlns="http://www.w3.org/2000/svg">
                    <path d="M3.612 15.443c-.386.198-.824-.149-.746-.592l.83-4.73L.173 6.765c-.329-.314-.158-.888.283-.95l4.898-.696L7.538.792c.197-.39.73-.39.927 0l2.184 4.327 4.898.696c.441.062.612.636.283.95l-3.523 3.356.83 4.73c.078.443-.36.79-.746.592L8 13.187l-4.389 2.256z"/>
                  </svg>
                  </span>
                  <span class="ml-2 rating-count">
                    3,840
                  </span>
                </div>

              </div>
            </div>

            <div id="talks"></div>
            <div class=" talks d-flex flex-row flex-wrap">

              
                <h2 class="w-100 section-header sticky-top">talks</h2>
             
              
                <div @mouseenter="talkEnter" @mouseleave="talkLeave" class="talk-card d-flex flex-column flex-grow-1 ">

                  <div class="">
                    <h4 class="card-heading">Frontend Love Meetup</h4>
                    <p class="talk-venue">Online</p>
                    <span class="date">November 4, 2020</span>
              
                  </div>

                  <div class="talk-topic mt-auto">
                    <h3>State Machines in Vue 3</h3>
                    <div class="mt-3">
                      <a class="mr-3">
                        Video
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" width="13" height="13" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 12 12" aria-hidden="true" class="flex-none stroke-current"><title>External link icon</title><path d="M10.976 1.193A.314.314 0 0010.687 1H6.312a.313.313 0 000 .625h3.62L5.467 6.091a.313.313 0 00.443.442l4.466-4.466v3.62a.313.313 0 00.625 0V1.313a.328.328 0 00-.024-.119z"></path><path d="M3.5 1v.625H2.25a.625.625 0 00-.625.625v7.5c0 .345.28.625.625.625h7.5c.345 0 .625-.28.625-.625V8.5H11v1.875c0 .345-.28.625-.625.625h-8.75A.625.625 0 011 10.375v-8.75C1 1.28 1.28 1 1.625 1H3.5z"></path></svg>
                      </a>
                      <a class="">
                        Slide
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" width="13" height="13" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 12 12" aria-hidden="true" class="flex-none stroke-current"><title>External link icon</title><path d="M10.976 1.193A.314.314 0 0010.687 1H6.312a.313.313 0 000 .625h3.62L5.467 6.091a.313.313 0 00.443.442l4.466-4.466v3.62a.313.313 0 00.625 0V1.313a.328.328 0 00-.024-.119z"></path><path d="M3.5 1v.625H2.25a.625.625 0 00-.625.625v7.5c0 .345.28.625.625.625h7.5c.345 0 .625-.28.625-.625V8.5H11v1.875c0 .345-.28.625-.625.625h-8.75A.625.625 0 011 10.375v-8.75C1 1.28 1.28 1 1.625 1H3.5z"></path></svg>
                      </a>
                      
                    </div>
                  </div>


                </div>
                <div @mouseenter="talkEnter" @mouseleave="talkLeave" class="talk-card d-flex flex-column flex-grow-1 ">

                  <div class="">
                    <h4 class="card-heading">Frontend Love Meetup</h4>
                    <p class="talk-venue">Amsterdam — The Netherlands</p>
                    <span class="date">November 4, 2020</span>
              
                  </div>

                  <div class="talk-topic mt-auto">
                    <h3>State Machines in Vue 3</h3>
                    <div class="mt-3">
                      <a class="mr-3">
                        Video
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" width="13" height="13" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 12 12" aria-hidden="true" class="flex-none stroke-current"><title>External link icon</title><path d="M10.976 1.193A.314.314 0 0010.687 1H6.312a.313.313 0 000 .625h3.62L5.467 6.091a.313.313 0 00.443.442l4.466-4.466v3.62a.313.313 0 00.625 0V1.313a.328.328 0 00-.024-.119z"></path><path d="M3.5 1v.625H2.25a.625.625 0 00-.625.625v7.5c0 .345.28.625.625.625h7.5c.345 0 .625-.28.625-.625V8.5H11v1.875c0 .345-.28.625-.625.625h-8.75A.625.625 0 011 10.375v-8.75C1 1.28 1.28 1 1.625 1H3.5z"></path></svg>
                      </a>
                      <a class="">
                        Slide
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" width="13" height="13" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 12 12" aria-hidden="true" class="flex-none stroke-current"><title>External link icon</title><path d="M10.976 1.193A.314.314 0 0010.687 1H6.312a.313.313 0 000 .625h3.62L5.467 6.091a.313.313 0 00.443.442l4.466-4.466v3.62a.313.313 0 00.625 0V1.313a.328.328 0 00-.024-.119z"></path><path d="M3.5 1v.625H2.25a.625.625 0 00-.625.625v7.5c0 .345.28.625.625.625h7.5c.345 0 .625-.28.625-.625V8.5H11v1.875c0 .345-.28.625-.625.625h-8.75A.625.625 0 011 10.375v-8.75C1 1.28 1.28 1 1.625 1H3.5z"></path></svg>
                      </a>
                      
                    </div>
                  </div>


                </div>
                <div @mouseenter="talkEnter" @mouseleave="talkLeave" class="talk-card d-flex flex-column flex-grow-1 ">

                  <div class="">
                    <h4 class="card-heading">Frontend Love Meetup</h4>
                    <p class="talk-venue">Online</p>
                    <span class="date">November 4, 2020</span>
              
                  </div>

                  <div class="talk-topic mt-auto">
                    <h3>State Machines in Vue 3</h3>
                    <div class="mt-3">
                      <a class="mr-3">
                        Video
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" width="13" height="13" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 12 12" aria-hidden="true" class="flex-none stroke-current"><title>External link icon</title><path d="M10.976 1.193A.314.314 0 0010.687 1H6.312a.313.313 0 000 .625h3.62L5.467 6.091a.313.313 0 00.443.442l4.466-4.466v3.62a.313.313 0 00.625 0V1.313a.328.328 0 00-.024-.119z"></path><path d="M3.5 1v.625H2.25a.625.625 0 00-.625.625v7.5c0 .345.28.625.625.625h7.5c.345 0 .625-.28.625-.625V8.5H11v1.875c0 .345-.28.625-.625.625h-8.75A.625.625 0 011 10.375v-8.75C1 1.28 1.28 1 1.625 1H3.5z"></path></svg>
                      </a>
                      <a class="">
                        Slide
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" width="13" height="13" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 12 12" aria-hidden="true" class="flex-none stroke-current"><title>External link icon</title><path d="M10.976 1.193A.314.314 0 0010.687 1H6.312a.313.313 0 000 .625h3.62L5.467 6.091a.313.313 0 00.443.442l4.466-4.466v3.62a.313.313 0 00.625 0V1.313a.328.328 0 00-.024-.119z"></path><path d="M3.5 1v.625H2.25a.625.625 0 00-.625.625v7.5c0 .345.28.625.625.625h7.5c.345 0 .625-.28.625-.625V8.5H11v1.875c0 .345-.28.625-.625.625h-8.75A.625.625 0 011 10.375v-8.75C1 1.28 1.28 1 1.625 1H3.5z"></path></svg>
                      </a>
                      
                    </div>
                  </div>


                </div>
                <div @mouseenter="talkEnter" @mouseleave="talkLeave" class="talk-card d-flex flex-column flex-grow-1 ">

                  <div class="">
                    <h4 class="card-heading">Frontend Love Meetup</h4>
                    <p class="talk-venue">Online</p>
                    <span class="date">November 4, 2020</span>
              
                  </div>

                  <div class="talk-topic mt-auto">
                    <h3>State Machines in Vue 3</h3>
                    <div class="mt-3">
                      <a class="mr-3">
                        Video
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" width="13" height="13" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 12 12" aria-hidden="true" class="flex-none stroke-current"><title>External link icon</title><path d="M10.976 1.193A.314.314 0 0010.687 1H6.312a.313.313 0 000 .625h3.62L5.467 6.091a.313.313 0 00.443.442l4.466-4.466v3.62a.313.313 0 00.625 0V1.313a.328.328 0 00-.024-.119z"></path><path d="M3.5 1v.625H2.25a.625.625 0 00-.625.625v7.5c0 .345.28.625.625.625h7.5c.345 0 .625-.28.625-.625V8.5H11v1.875c0 .345-.28.625-.625.625h-8.75A.625.625 0 011 10.375v-8.75C1 1.28 1.28 1 1.625 1H3.5z"></path></svg>
                      </a>
                      <a class="">
                        Slide
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" width="13" height="13" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 12 12" aria-hidden="true" class="flex-none stroke-current"><title>External link icon</title><path d="M10.976 1.193A.314.314 0 0010.687 1H6.312a.313.313 0 000 .625h3.62L5.467 6.091a.313.313 0 00.443.442l4.466-4.466v3.62a.313.313 0 00.625 0V1.313a.328.328 0 00-.024-.119z"></path><path d="M3.5 1v.625H2.25a.625.625 0 00-.625.625v7.5c0 .345.28.625.625.625h7.5c.345 0 .625-.28.625-.625V8.5H11v1.875c0 .345-.28.625-.625.625h-8.75A.625.625 0 011 10.375v-8.75C1 1.28 1.28 1 1.625 1H3.5z"></path></svg>
                      </a>
                      
                    </div>
                  </div>


                </div>

            </div>

            <div id="interviews"></div>
            <div class="interview">
              <h2 class="section-header sticky-top">interview</h2>
              <div @mouseenter="interviewEnter" @mouseleave="interviewLeave" class="interview-col"> 
                <a href="#">
                <div class="interview-card d-flex flex-row">
                  <div class="play-button d-flex justify-content-center align-items-center">
              
                    <svg width="45" height="45" viewBox="0 0 16 16" class="bi bi-play" fill="currentColor" xmlns="http://www.w3.org/2000/svg">
                      <path fill-rule="evenodd" d="M10.804 8L5 4.633v6.734L10.804 8zm.792-.696a.802.802 0 0 1 0 1.392l-6.363 3.692C4.713 12.69 4 12.345 4 11.692V4.308c0-.653.713-.998 1.233-.696l6.363 3.692z"/>
                    </svg>
                  </div>

                  <div class="details">
                    <h3>Live Coding</h3>
                    <p class="mt-8 mb-2">
                      <span itemprop="publisher">
                        DreamStacks Podcast
                      </span> — with
                      <span itemprop="author">
                        Amelia Winger-Bearskin, Sam Agnew, Dan Gorelick, Shy Ruparel
                      </span>
                    </p>
                    <p class="time">
                      setember 4, 2020
                    </p>
                  </div>

                </div>
                </a>
              </div>
              <div @mouseenter="interviewEnter" @mouseleave="interviewLeave" class="interview-col"> 
                <a href="#">
                <div class="interview-card d-flex flex-row">
                  <div class="play-button d-flex justify-content-center align-items-center">
              
                    <svg width="45" height="45" viewBox="0 0 16 16" class="bi bi-play" fill="currentColor" xmlns="http://www.w3.org/2000/svg">
                      <path fill-rule="evenodd" d="M10.804 8L5 4.633v6.734L10.804 8zm.792-.696a.802.802 0 0 1 0 1.392l-6.363 3.692C4.713 12.69 4 12.345 4 11.692V4.308c0-.653.713-.998 1.233-.696l6.363 3.692z"/>
                    </svg>
                  </div>

                  <div class="details">
                    <h3>Live Coding</h3>
                    <p class="mt-8 mb-2">
                      <span itemprop="publisher">
                        DreamStacks Podcast
                      </span> — with
                      <span itemprop="author">
                        Amelia Winger-Bearskin, Sam Agnew, Dan Gorelick, Shy Ruparel
                      </span>
                    </p>
                    <p class="time">
                      setember 4, 2020
                    </p>
                  </div>

                </div>
                </a>
              </div>
              <div @mouseenter="interviewEnter" @mouseleave="interviewLeave" class="interview-col"> 
                <a href="#">
                <div class="interview-card d-flex flex-row">
                  <div class="play-button d-flex justify-content-center align-items-center">
              
                    <svg width="45" height="45" viewBox="0 0 16 16" class="bi bi-play" fill="currentColor" xmlns="http://www.w3.org/2000/svg">
                      <path fill-rule="evenodd" d="M10.804 8L5 4.633v6.734L10.804 8zm.792-.696a.802.802 0 0 1 0 1.392l-6.363 3.692C4.713 12.69 4 12.345 4 11.692V4.308c0-.653.713-.998 1.233-.696l6.363 3.692z"/>
                    </svg>
                  </div>

                  <div class="details">
                    <h3>Live Coding</h3>
                    <p class="mt-8 mb-2">
                      <span itemprop="publisher">
                        DreamStacks Podcast
                      </span> — with
                      <span itemprop="author">
                        Amelia Winger-Bearskin, Sam Agnew, Dan Gorelick, Shy Ruparel
                      </span>
                    </p>
                    <p class="time">
                      setember 4, 2020
                    </p>
                  </div>

                </div>
                </a>
              </div>
              <div @mouseenter="interviewEnter" @mouseleave="interviewLeave" class="interview-col"> 
                <a href="#">
                <div class="interview-card d-flex flex-row">
                  <div class="play-button d-flex justify-content-center align-items-center">
              
                    <svg width="45" height="45" viewBox="0 0 16 16" class="bi bi-play" fill="currentColor" xmlns="http://www.w3.org/2000/svg">
                      <path fill-rule="evenodd" d="M10.804 8L5 4.633v6.734L10.804 8zm.792-.696a.802.802 0 0 1 0 1.392l-6.363 3.692C4.713 12.69 4 12.345 4 11.692V4.308c0-.653.713-.998 1.233-.696l6.363 3.692z"/>
                    </svg>
                  </div>

                  <div class="details">
                    <h3>Live Coding</h3>
                    <p class="mt-8 mb-2">
                      <span itemprop="publisher">
                        DreamStacks Podcast
                      </span> — with
                      <span itemprop="author">
                        Amelia Winger-Bearskin, Sam Agnew, Dan Gorelick, Shy Ruparel
                      </span>
                    </p>
                    <p class="time">
                      setember 4, 2020
                    </p>
                  </div>

                </div>
                </a>
              </div>
              <div @mouseenter="interviewEnter" @mouseleave="interviewLeave" class="interview-col"> 
                <a href="#">
                <div class="interview-card d-flex flex-row">
                  <div class="play-button d-flex justify-content-center align-items-center">
              
                    <svg width="45" height="45" viewBox="0 0 16 16" class="bi bi-play" fill="currentColor" xmlns="http://www.w3.org/2000/svg">
                      <path fill-rule="evenodd" d="M10.804 8L5 4.633v6.734L10.804 8zm.792-.696a.802.802 0 0 1 0 1.392l-6.363 3.692C4.713 12.69 4 12.345 4 11.692V4.308c0-.653.713-.998 1.233-.696l6.363 3.692z"/>
                    </svg>
                  </div>

                  <div class="details">
                    <h3>Live Coding</h3>
                    <p class="mt-8 mb-2">
                      <span itemprop="publisher">
                        DreamStacks Podcast
                      </span> — with
                      <span itemprop="author">
                        Amelia Winger-Bearskin, Sam Agnew, Dan Gorelick, Shy Ruparel
                      </span>
                    </p>
                    <p class="time">
                      setember 4, 2020
                    </p>
                  </div>

                </div>
                </a>
              </div>
              <div @mouseenter="interviewEnter" @mouseleave="interviewLeave" class="interview-col"> 
                <a href="#">
                <div class="interview-card d-flex flex-row">
                  <div class="play-button d-flex justify-content-center align-items-center">
              
                    <svg width="45" height="45" viewBox="0 0 16 16" class="bi bi-play" fill="currentColor" xmlns="http://www.w3.org/2000/svg">
                      <path fill-rule="evenodd" d="M10.804 8L5 4.633v6.734L10.804 8zm.792-.696a.802.802 0 0 1 0 1.392l-6.363 3.692C4.713 12.69 4 12.345 4 11.692V4.308c0-.653.713-.998 1.233-.696l6.363 3.692z"/>
                    </svg>
                  </div>

                  <div class="details">
                    <h3>Live Coding</h3>
                    <p class="mt-8 mb-2">
                      <span itemprop="publisher">
                        DreamStacks Podcast
                      </span> — with
                      <span itemprop="author">
                        Amelia Winger-Bearskin, Sam Agnew, Dan Gorelick, Shy Ruparel
                      </span>
                    </p>
                    <p class="time">
                      setember 4, 2020
                    </p>
                  </div>

                </div>
                </a>
              </div>
              

              
              <!-- <a href="#" @mouseenter="interviewEnter" @mouseleave="interviewLeave" class="a">
                <div class="interview-card d-flex flex-row">
                  <div class="play-button d-flex justify-content-center align-items-center">
              
                    <svg width="45" height="45" viewBox="0 0 16 16" class="bi bi-play" fill="currentColor" xmlns="http://www.w3.org/2000/svg">
                      <path fill-rule="evenodd" d="M10.804 8L5 4.633v6.734L10.804 8zm.792-.696a.802.802 0 0 1 0 1.392l-6.363 3.692C4.713 12.69 4 12.345 4 11.692V4.308c0-.653.713-.998 1.233-.696l6.363 3.692z"/>
                    </svg>
                  </div>

                  <div class="details">
                    <h3>Live Coding</h3>
                    <p class="mt-8 mb-2">
                      <span itemprop="publisher">
                        DreamStacks Podcast
                      </span> — with
                      <span itemprop="author">
                        Amelia Winger-Bearskin, Sam Agnew, Dan Gorelick, Shy Ruparel
                      </span>
                    </p>
                    <p class="time">
                      setember 4, 2020
                    </p>
                  </div>

                </div>
              </a>
              <a href="#" @mouseenter="interviewEnter" @mouseleave="interviewLeave" class="a">
                <div class="interview-card d-flex flex-row">
                  <div class="play-button d-flex justify-content-center align-items-center">
              
                    <svg width="45" height="45" viewBox="0 0 16 16" class="bi bi-play" fill="currentColor" xmlns="http://www.w3.org/2000/svg">
                      <path fill-rule="evenodd" d="M10.804 8L5 4.633v6.734L10.804 8zm.792-.696a.802.802 0 0 1 0 1.392l-6.363 3.692C4.713 12.69 4 12.345 4 11.692V4.308c0-.653.713-.998 1.233-.696l6.363 3.692z"/>
                    </svg>
                  </div>

                  <div class="details">
                    <h3>Live Coding</h3>
                    <p class="mt-8 mb-2">
                      <span itemprop="publisher">
                        DreamStacks Podcast
                      </span> — with
                      <span itemprop="author">
                        Amelia Winger-Bearskin, Sam Agnew, Dan Gorelick, Shy Ruparel
                      </span>
                    </p>
                    <p class="time">
                      setember 4, 2020
                    </p>
                  </div>

                </div>
              </a>
              <a href="#" @mouseenter="interviewEnter" @mouseleave="interviewLeave" class="a">
                <div class="interview-card d-flex flex-row">
                  <div class="play-button d-flex justify-content-center align-items-center">
              
                    <svg width="45" height="45" viewBox="0 0 16 16" class="bi bi-play" fill="currentColor" xmlns="http://www.w3.org/2000/svg">
                      <path fill-rule="evenodd" d="M10.804 8L5 4.633v6.734L10.804 8zm.792-.696a.802.802 0 0 1 0 1.392l-6.363 3.692C4.713 12.69 4 12.345 4 11.692V4.308c0-.653.713-.998 1.233-.696l6.363 3.692z"/>
                    </svg>
                  </div>

                  <div class="details">
                    <h3>Live Coding</h3>
                    <p class="mt-8 mb-2">
                      <span itemprop="publisher">
                        DreamStacks Podcast
                      </span> — with
                      <span itemprop="author">
                        Amelia Winger-Bearskin, Sam Agnew, Dan Gorelick, Shy Ruparel
                      </span>
                    </p>
                    <p class="time">
                      setember 4, 2020
                    </p>
                  </div>

                </div>
              </a> -->

            </div>

          </div>
          
        </div>

      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'home',
  data(){
    return{
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
   talkEnter(e){
     e.target.parentElement.querySelectorAll('.talk-card').forEach(card => {
      card.style.opacity = '0.5'
    });
    e.target.style.opacity = '1'  
   },
   talkLeave(e){
      e.target.parentElement.querySelectorAll('.talk-card').forEach(card => {
      card.style.opacity = '1'
    });
   },
   interviewEnter(e){
     e.target.parentElement.querySelectorAll('.interview-col').forEach(card => {
      card.style.opacity = '0.5'
    });
    e.target.style.opacity = '1'
    
   },
   interviewLeave(e){
     e.target.parentElement.querySelectorAll('.interview-col').forEach(card => {
      card.style.opacity = '1'
    });
   }
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
.talks{
  margin-top: 90px;
}
.talk-card{
  padding: 40px;
   --bg-opacity: 1;
    background-color: #202022;
    background-color: rgba(32,32,34,var(--bg-opacity));
    transition: all .3s ease;
    margin-bottom: 10px;
    width: 270px;
    margin: 5px;
    min-height: 340px;
    transition: all .2s ease;
}
.talk-card:hover{
  transform: scale(1.15);
}
.talk-venue, .date{
  color: rgb(148, 148, 149);
  margin-bottom: 0px;
}
.talk-topic a{
  cursor: pointer;
  color: white;
  text-decoration: none;
}
.talk-topic svg{
  color: rgb(148, 148, 149);
}
/*  */
.interview{
  margin-top: 100px;
}
.interview a{
  text-decoration: none;
  
}
.interview-card {
  margin: 48px 0px;
}

.play-button{
  min-height: 120px;
  min-width: 120px;
  border-radius: 50%;
  background-color: red;
  margin-right: 40px;
  --bg-opacity: 1;
    background-color: #202022;
    background-color: rgba(32,32,34,var(--bg-opacity));
    color: white;
    transition: all 0.3s ease;
}
.interview-card:hover .play-button{
  transform: scale(1.1);
}
.details h3{
  font-size: 24px;
  color: white;
  line-height: 1.25;
  font-weight: 600;
}
.details p{
   color: rgb(148, 148, 149);
}
.details .time{
  letter-spacing: 3px;
  text-transform: uppercase;
  margin-top: 8px;
  font-weight: bold;
  color: white;
  font-size: 10px;
}

@media (min-width: 1200px) { 
  .container{
      max-width: 1250px !important;
  }
 }

@media (max-width: 1199.98px) {  }
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
  .mobile_top{
    display: inline-block;
    height: 60px;
    background-color: #202022;
  }
 }

@media (max-width: 767.98px) { 
  .play-button{
    min-width: 120px;
    min-height: 0px;
    height: 120px;
    margin-right: 30px;
  }
  
 }
@media (max-width: 575.98px) {  }

</style>
