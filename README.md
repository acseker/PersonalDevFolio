<h1 align="center">PersonalDevFolio</h1>

<div align="center">


  ![GitHub deployments](https://img.shields.io/github/deployments/acseker/PersonalDevFolio/github-pages?label=Deploy&logo=github&style=for-the-badge)

</div>

This repo is a personal developer portfolio and a modified version of [DevFolio](https://github.com/AnilSeervi/DevFolio) repo.
If you would like to use this portfolio, please follow the instructions in it.

To view a **[live](https://acseker.github.io/PersonalDevFolio/)** example of PersonalDevFolio.

---
## Template Structure
This portfolio consists of `index.html`, `projectX.html` files in `projects` folder
and `main.css` file in `css` folder.

The `.html` files consist of the following sections:
* Head
* Bar
* Hero
* About
* Skills
* Projects
* Tools
* Awards
* Publications
* Contact
* Footer


### Head Section
- Add a title to your Portfolio website within the `<title>` tag.
- Add some keywords and description to your Portfolio website as directed in the `index.html` file.

```html
<!-- Title: add your Portfolio websites's title here -->
<title>[Your name here] | Developer</title>
<!-- Add some coding keywords below, Ex: (javascript, yourusername, etc) -->
<meta name="keywords" content="[username], [name], skill" />
<!-- Improve your SEO by adding a small descrption of you -->
<meta name="description" content="[Your name here] | Developer" />
```


### Bar Section
* On `.dropdown-content`, put your custom project name.

```html
  <!-- Top Navigation Bar Section -->
  <div id="bar">
    <div class="navbar">
  
      <a href="#hero">
        <img src="../assets/icon.png" height="20px" alt="Icon Image">
      </a>
  
      <div class="navbar-titles">
        <a href="#hero">Home</a>
        <a href="#about">About Me</a>
        <a href="#skills">Skills</a>
  
        <div class="dropdown">
          <button class="dropbtn">
            Projects <i class="fa fa-caret-down"></i>
          </button>
          <div class="dropdown-content">
            <a href="projects/project1.html">Project Name</a>
            <a href="projects/project2.html">Project Name</a>
            <a href="projects/project3.html">Project Name</a>
            <a href="projects/project4.html">Project Name</a>
          </div>
        </div>
  
        <a href="#awards">Awards</a>
        <a href="#publications">Publications</a>
        <a href="#contact">Contact</a>
      </div>
    </div>
  </div>
  <!-- /END Top Navigation Bar Section -->
```


### Hero Section
- On `.hero-title`, put your custom title.
- On `.hero-subtitle`, put your custom subtitles.
- On `social-links`, put your social link url on `href` attribute   

```html
    <!-- Hero Section -->
    <div id="hero">
      <section class="container">
        <h1 class="hero-title">
          Hi! <br> I'm Ahmet Cagatay Seker
        </h1>

        <h1 class="hero-subtitle">
           Ph.D. Candidate | Junior ML Developer | Research Assistant
        </h1>
        <br>

        <div class="social-links">
          <a
            href="mailto:acseker07@gmail.com"
            target="_blank"
            rel="noopener noreferrer"
            aria-label="email"
          >
            <span class="fa-stack" style="vertical-align: top;">
              <i class="fa fa-circle fa-stack-2x" style="color:#ea4335"></i>
              <i class="fa fa-envelope fa-stack-1x"></i>
            </span>
          </a>

          <a
            href="https://www.linkedin.com/in/acseker/"
            target="_blank"
            rel="noopener noreferrer"
            aria-label="linkedin"
          >
            <span class="fa-stack" style="vertical-align: top;">
              <i class="fa fa-circle fa-stack-2x" style="color:#4875b4"></i>
              <i class="fa fa-linkedin fa-stack-1x"></i>
            </span>
          </a>

          <a
            href="https://github.com/acseker"
            target="_blank"
            rel="noopener noreferrer"
            aria-label="github"
          >
            <span class="fa-stack" style="vertical-align: top;">
              <i class="fa fa-circle fa-stack-2x" style="color:#000"></i>
              <i class="fa fa-github fa-stack-1x"></i>
            </span>
          </a>
        </div>
      </section>

      <a href="#about" class="scroll-down-link" aria-label="scroll-down">
        <div class="scroll-down"></div>
      </a>
    </div>
    <!-- /END Hero Section -->
```


### About Section
- On `<img>` tag, fill the `src` attribute with your profile picture, your picture must be located inside `assets/` folder.
  - Recommended size for your profile image is (450 x 450px).
- On `<p>` tag with class-name `.about-wrapper__info-text`, include information about you, I recommend to use 2 paragraphs in order to work well and a maximum of 3 paragraphs.
- On last `<a>` tag, include your resume url on `href` attribute.

```html
<!-- About Section -->
<section id="about">
  <div class="container">
    <h2 class="section-title">About Me</h2>
    <div class="row about-wrapper">
      <div class="about-wrapper__image">
        <img class="img-fluid" src="./assets/profile.png" alt="Profile Image" />
      </div>
      <div class="about-wrapper__info">
        <p class="about-wrapper__info-text">
          Lorem ipsum dolor sit amet consectetur adipisicing elit.
        </p>
        <p class="about-wrapper__info-text">
          Lorem ipsum dolor sit amet consectetur adipisicing elit.
        </p>
        <span class="about-wrapper__cta">
          <a href="#" class="cta-btn cta-btn--resume">View Resume</a>
        </span>
      </div>
    </div>
  </div>
</section>
<!-- /END About Section -->
```


### Skills Section
- On `<img>` tag, fill the `src` attribute with your skill picture.

```html
<!-- Skills Section -->
<section id="skills">
  <div class="container">
    <div class="skills-wrapper">
      <h2 class="section-title dark-blue-text">Skills</h2>
        <div class="skills-wrapper__text">
          <div style="padding-left:25px">
            <img src="./assets/python.png" height="64px"/>
            <h6>Python</h6>
          </div>
          <div style="padding-left:25px">
            <img src="./assets/c++.png" height="64px"/>
            <h6>C++</h6>
          </div>
          <div style="padding-left:25px">
            <img src="./assets/html.png" height="64px"/>
            <h6>HTML</h6>
          </div>
          <div style="padding-left:25px">
            <img src="./assets/css.png" height="64px"/>
            <h6>CSS</h6>
          </div>
        </div>
      </div>
  </div>
</section>
<!-- /END Skill Section -->
```


### Projects Section
- Each project lives inside `row` class.
- On `<h3>` tag with class-name `.project-wrapper__text-title`, include your project title.
- On `<p>` tag with `loremp ipsum` text, include your project information.
- On first `<a>` tag, put your project url on `href` attribute.
- On second `<a>` tag, put your project repository url on `href` attribute.
- Inside `<div>` tag with class-name `.project-wrapper__image`, 
  - put your project image url on the `src` of the `<img>` 
  - put again your project url on `href` attribute of `<a>` tag.
- Recommended size for project image (1366 x 767px), your project image must live in `assets/` folder. 
- 
```html
<!--Projects Section-->
    <section id="projects">
      <div class="container">
        <div class="project-wrapper">
          <h2 class="section-title dark-blue-text">Projects</h2>

        <!-- Each .row is a project -->
          <div class="row">
            <div class="project-wrapper__text">
              <h3 class="project-wrapper__text-title">Project Title</h3>
              <p class="project-wrapper__text-info">
                Lorem ipsum dolor sit amet consectetur adipisicing elit.
              </p>
              <div class="project-wrapper__text-btns">
                <a
                  href="#"
                  target="_blank"
                  class="cta-btn cta-btn--hero cta-btn--projects"
                  >See Live</a
                >
                <a href="#" target="_blank" class="cta-btn text-color-main"
                  >Source Code</a
                >
              </div>
            </div>

            <div class="project-wrapper__image">
              <a href="#" target="_blank">
                <div class="thumbnail rounded">
                  <img
                    src="./assets/project.png"
                    class="img-fluid"
                    alt="Project Image"
                  />
                </div>
              </a>
            </div>
          </div>
          ...
          </section>
<!-- /END Project -->
```


### Tools
- On `<img>` tag, fill the `src` attribute with your skill picture.

```html
<!-- tools Section -->
<section id="tools">
  <div class="container">
    <div class="tools-wrapper">
      <h2 class="section-title dark-blue-text">Tools</h2>
        <div class="tools-wrapper__text">
          <div style="padding-left:25px">
            <img src="../assets/python.png" height="64px"/>
            <h6>Python</h6>
          </div>
          <div style="padding-left:25px">
            <img src="../assets/pytorch.png" height="64px"/>
            <h6>PyTorch</h6>
          </div>
          <div style="padding-left:25px">
            <img src="../assets/opencv.png" height="64px"/>
            <h6>OpenCV</h6>
          </div>              
        </div>
      </div>
    </div>
</section>
<!-- /END Skill Section -->
```


### Awards Section
- On `<h3>` tag with class-name `.project-wrapper__text-title`, include your project title.
- On `<p>` tag with the text, include your awards information.

```html
<!-- Awards Section -->
<section id="awards">
  <div class="container">
    <div class="awards-wrapper">
      <h2 class="section-title dark-blue-text">Awards</h2>
      <div class="awards-wrapper__text">
        <p class="awards-wrapper__text-info">
          🏆 Graduated as the highest ranked student
          in the Faculty of Engineering at Mevlana University in Jun 2015.
        </p>
      </div>
    </div>
  </div>
</section>
<!-- /END Awards Section -->
```


### Publications Section
- On `<h3>` tag with class-name `.project-wrapper__text-title`, include your project title.
- On `<p>` tag with the text, include your awards information.

```html
<!-- Publications Section -->
<section id="publications">
  <div class="container">
    <div class="publications-wrapper">
      <h2 class="section-title dark-blue-text">Publications</h2>
      <div class="publications-wrapper__text">
        <p class="publications-wrapper__text-info">
          📃 A Generalized Framework for Recognition of Expiration Date on Product Packages Using Fully Convolutional Networks
          <br>
          Seker, Ahmet Cagatay and Ahn, Sang Chul
        </p>
      </div>
    </div>
  </div>
</section>
<!-- /END Publications Section -->
```


### Contact Section
- On `<p>` tag with class-name `.contact-wrapper__text`, include some custom call-to-action message.
- On `<a>` tag, put your email address on `action="your-mail-address` attribute.

```html
<!-- Contact Section -->
<section id="contact">
  <div class="container">
    <h2 class="section-title">Contact</h2>
    <div class="contact-wrapper">
      <div id="contact-form">
        <form method="POST" action="https://formspree.io/acseker07@gmail.com">
            <input type="hidden" name="_subject" value="Contact request from personal website">
            <input type="email" name="_replyto" placeholder="Your email" required="">
            <textarea name="message" placeholder="Your message" required="" data-gramm="false" wt-ignore-input="true"></textarea>
            <button class="cta-btn cta-btn--resume" type="submit">Submit</button>
        </form>
      </div>
    </div>
  </div>
</section>
<!-- END Contact Section -->
```


### Footer Section
- Put your social media link on each `<a>` links.
- If you have more social-media accounts, see [Font Awesome Icons](https://fontawesome.com/v4.7.0/icons/) to put the corresponding additional social icon classNames.
- You can delete or add as many `a` links your want.

```html
<!-- Footer Section -->
<footer class="footer">
  ...
  <div class="social-links">
    </a>
    <a href="#!" target="_blank">
      <i class="fa fa-linkedin"></i>
    </a>
    <a href="#!" target="_blank">
      <i class="fa fa-github"></i>
    </a>
  </div>
  ...
</footer>
<!-- END Footer Section -->
```





