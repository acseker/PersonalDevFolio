<h1 align="center">PersonalDevFolio</h1>

<div align="center">
adresi degistir

  ![GitHub deployments](https://img.shields.io/github/deployments/anilseervi/DevFolio/github-pages?label=Deploy&logo=github&style=for-the-badge)

</div>

This repo is a personal developer portfolio and a modified version of [DevFolio](https://github.com/AnilSeervi/DevFolio).
If you would like to use this portfolio, please follow the instructions in it.

To view a **[live](https://acseker.github.io/PersonalDevFolio/)** example of PersonalDevFolio.

---
## Template Structure
This portfolio consists of the main and the project pages.

The main page consists of the following sections:
* Hero
* About
* Skills
* Projects
* Awards
* Publications
* Contact
* Footer

Project pages consists of the following sections:
* Hero
* Projects
* Tools
* Contact
* Footer


Open `index.html` for the main page and fill your information, there are 6 sections:

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

- Remove google analytics tag before pushing it to GitHub.

### Hero Section
- On `.hero-title`, put your custom title.
- On `.hero-cta`, put your custom button cta.

```html
<!-- Hero Section -->
<div id="hero">
  <section class="container">
    <h1 class="hero-title">
      Hi, my name is <span class="text-color-main name">Your Name</span>
      <br />
      I'm the Unknown Developer.
    </h1>
    <p class="hero-cta">
      <a class="cta-btn cta-btn--hero" href="#about">Get in touch</a>
    </p>
  </section>
  <a href="#about" class="scroll-down-link"> <div class="scroll-down"></div></a>
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


### Projects Section
- Each project lives inside `row` class.
- On `<h3>` tag with class-name `.project-wrapper__text-title`, include your project title.
- On `<p>` tag with `loremp ipsum` text, include your project information.
- On first `<a>` tag, put your project url on `href` attribute.
- On second `<a>` tag, put your project repository url on `href` attribute.

---

- Inside `<div>` tag with class-name `.project-wrapper__image`, put your project image url on the `src` of the `<img>` and put again your project url on `href` attribute of `<a>` tag.
- Recommended size for project image (1366 x 767px), your project image must live in `assets/` folder. You can remove the default images and replace them with yours.

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

### Awards Section

### Publications Section

### Tools Section


### Contact Section
- On `<p>` tag with class-name `.contact-wrapper__text`, include some custom call-to-action message.
- On `<a>` tag, put your email address on `href="mailto:` attribute.

```html
<!-- Contact Section -->
<section id="contact">
  <div class="container">
    <h2 class="section-title">Contact</h2>
    <div class="contact-wrapper">
      <p class="contact-wrapper__text">[Put your call to action here]</p>
      <a href="mailto:" class="cta-btn cta-btn--resume">Call to Action</a>
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
    <a href="#!" target="_blank">
      <i class="fa fa-twitter"></i>
    </a>
    <a href="#!" target="_blank">
      <i class="fa fa-instagram"></i>
    </a>
    <a href="#!" target="_blank">
      <i class="fa fa-codepen"></i>
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




