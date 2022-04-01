# Frontend Mentor - Testimonials grid section solution

This is a solution to the [Testimonials grid section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

### Screenshot

![](./design/desktop-design.jpg)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

This project really improved and strenghtened my knowledge on CSS Grid

To see how you can add code snippets, see below:

```html
<article class="testimonial testimonial-1 grid-col-span-2">
    <div class="flex">
      <div class="img">
        <img src="dist/images/image-daniel.jpg" alt="" srcset="" class="img-1">
      </div>
      <div>
        <h2 class="name">Daniel Clifford</h2>
        <p class="position">Verified Graduate</p>
      </div>
      
    </div>
    
    <h3>I received a job offer mid-course, and the subjects I learned were current, if not more so, 
      in the company I joined. I honestly feel I got every penny’s worth.
    </h3>
      <p>
        “ I was an EMT for many years before I joined the bootcamp. I’ve been looking to make a 
        transition and have heard some people who had an amazing experience here. I signed up 
        for the free intro course and found it incredibly fun! I enrolled shortly thereafter. 
        The next 12 weeks was the best - and most grueling - time of my life. Since completing 
        the course, I’ve successfully switched careers, working as a Software Engineer at a VR startup. ”
      </p>

      <img src="dist/images/bg-pattern-quotation.svg" alt="bg-pattern-quotation" class="quotation">
   
  </article>

  <article class="testimonial testimonial-2">
    <div class="flex">
      <div class="img">
        <img src="dist/images/image-jonathan.jpg" alt="" class="img-2">
      </div>
      <div>
        <h2 class="name">Jonathan Walters</h2>
        <p class="position">Verified Graduate</p>
      </div>
      
    </div>

  <h3>
    The team was very supportive and kept me motivated
  </h3>

  <p>“ I started as a total newbie with virtually no coding skills. I now work as a mobile engineer 
    for a big company. This was one of the best investments I’ve made in myself. ”</p>
  </article>

  <article class="testimonial testimonial-3">
    <div class="flex">
      <div class="img">
        <img src="dist/images/image-jeanette.jpg" alt="" srcset="" class="img-3">
      </div>
      <div>
        <h2 class="name">Jeanette Harmon</h2>
        <p class="position">Verified Graduate</p>
      </div>
      
    </div>

  <h3>An overall wonderful and rewarding experience</h3>

  <p>“ Thank you for the wonderful experience! I now have a job I really enjoy, and make a good living 
    while doing something I love. ”</p>
  </article>

  <article class="testimonial testimonial-4 grid-col-span-2">
    <div class="flex">
      <div class="img">
        <img src="dist/images/image-patrick.jpg" alt="" class="img-4">
      </div>
      <div>
        <h2 class="name">Patrick Abrams</h2>
        <p class="position">Verified Graduate</p>
      </div>
      
    </div>

  <h3>Awesome teaching support from TAs who did the bootcamp themselves. Getting guidance from them and 
    learning from their experiences was easy.</h3>

  <p>“ The staff seem genuinely concerned about my progress which I find really refreshing. The program 
    gave me the confidence necessary to be able to go out in the world and present myself as a capable 
    junior developer. The standard is above the rest. You will get the personal attention you need from 
    an incredible community of smart and amazing people. ”</p>
  </article>

  <article class="testimonial testimonial-5">
    <div class="flex">
      <div class="img">
        <img src="dist/images/image-kira.jpg" alt="" class="img-5">
      </div>
      <div>
        <h2 class="name">Kira Whittle</h2>
        <p class="position">Verified Graduate</p>
      </div>
      
    </div>

  <h3>Such a life-changing experience. Highly recommended!</h3>

  <p>“ Before joining the bootcamp, I’ve never written a line of code. I needed some structure from 
    professionals who can help me learn programming step by step. I was encouraged to enroll by a former 
    student of theirs who can only say wonderful things about the program. The entire curriculum and staff 
    did not disappoint. They were very hands-on and I never had to wait long for assistance. The agile team 
    project, in particular, was outstanding. It took my learning to the next level in a way that no tutorial 
    could ever have. In fact, I’ve often referred to it during interviews as an example of my developent 
    experience. It certainly helped me land a job as a full-stack developer after receiving multiple offers. 
    100% recommend! ”</p>
  </article>
```
```css
.testimonial-grid {
    padding: 30px;


    display: grid;
    gap: 30px;
    grid-auto-columns: 1fr;
    grid-template-areas: 
    'one'
    'two'
    'three'
    'four'
    'five';
}

.testimonial-1 {
        background: hsl(263, 55%, 52%);
        grid-area: one;
        position: relative;
        z-index: 1;
}

.testimonial-2 {
        background: hsl(217, 19%, 35%);
        grid-area: two;
    }
.testimonial-3 {
        background: hsl(0, 0%, 100%);
        color: hsl(217, 19%, 35%);
        grid-area: three;
    }
.testimonial-4 {
        background: hsl(219, 29%, 14%);
        grid-area: four;
    }
.testimonial-5 {
        background: hsl(0, 0%, 100%);
        color: hsl(217, 19%, 35%);
        grid-area: five;
    }

    @media (min-width: 35em) {
    .testimonial-grid {
        grid-template-areas: 
        'one one'
        'two five'
        'three five'
        'four four';
    }
}

@media (min-width: 50em) {
    .testimonial-grid {
        grid-template-areas: 
        'one one two five'
        'three four four five';
    }
}
```

### Continued development

Working on more projects with CSS Grid

### Useful resources

- [Kevil Powell's CSS Grid Tutorial]()

## Author

- Website - [Daniel Okafor](https://www.your-site.com)
- Frontend Mentor - [@Buch-dev](https://www.frontendmentor.io/profile/Buch-dev)
- Twitter - [@bucheed](https://www.twitter.com/bucheed)
