<template>
  <div class="content">
    <div class="md-layout">
      <div class="md-layout-item md-medium-size-100 md-size-66">
        <!--<edit-profile-form data-background-color="green"> </edit-profile-form> -->
        <content-header data-background-color="Lavender"></content-header>
      </div>
      <div class="md-layout-item md-medium-size-100 md-size-33">
        <md-button class="md-sm md-simple"
          >Email
          <v-btn flat color="yellow"></v-btn>
        </md-button>

        <user-card>
          <md-card class="md-card-profile">
            <div class="md-card-avatar">
              <img class="img" :src="cardUserImage" />
            </div>
            <md-card-content>
              <h6 class="category text-gray">Software Engineer</h6>
              <h4 class="card-title">Garikai T Matanhatu</h4>
              <p class="card-description">
                To focus on the visible at the expense of the essential is
                irresponsible....
              </p>
              <!-- <md-button class="md-round md-success">Follow</md-button>-->
            </md-card-content>
          </md-card>
        </user-card>
        <user-profile>
          <!-- Portfolio Grid-->
          <md-card>
            <md-card-header data-background-color="silver">
              <h4 class="title">PORTFOLIO</h4>
            </md-card-header>
            <section class="page-section bg-light" id="portfolio">
              <div class="container">
                <div class="text-center">
                  <h2 class="section-heading text-uppercase">PORTFOLIO</h2>
                  <h3 class="section-subheading text-muted">
                    This is my Portfolio.
                  </h3>
                </div>
                <div class="row">
                  <div class="col-lg-4 col-sm-6 mb-4">
                    <!-- Portfolio item 1-->
                    <div class="portfolio-item">
                      <a
                        class="portfolio-link"
                        data-bs-toggle="modal"
                        href="#portfolioModal1"
                      >
                        <div class="portfolio-hover">
                          <div class="portfolio-hover-content">
                            <i class="fas fa-plus fa-3x"></i>
                          </div>
                        </div>
                        <img
                          class="img-fluid"
                          src="assets/img/portfolio/1.jpg"
                          alt="..."
                        />
                      </a>
                      <div class="portfolio-caption">
                        <div class="portfolio-caption-heading">Project</div>
                        <div class="portfolio-caption-subheading text-muted">
                          Java
                        </div>
                      </div>
                    </div>
                  </div>
                  <div class="col-lg-4 col-sm-6 mb-4">
                    <!-- Portfolio item 2-->
                    <div class="portfolio-item">
                      <a
                        class="portfolio-link"
                        data-bs-toggle="modal"
                        href="#portfolioModal2"
                      >
                        <div class="portfolio-hover">
                          <div class="portfolio-hover-content">
                            <i class="fas fa-plus fa-3x"></i>
                          </div>
                        </div>
                        <img
                          class="img-fluid"
                          src="assets/img/portfolio/2.jpg"
                          alt="..."
                        />
                      </a>
                      <div class="portfolio-caption">
                        <div class="portfolio-caption-heading">Explore</div>
                        <div class="portfolio-caption-subheading text-muted">
                          VUE.JS
                        </div>
                      </div>
                    </div>
                  </div>
                  <div class="col-lg-4 col-sm-6 mb-4"></div>
                </div>
              </div>
            </section>
          </md-card>
        </user-profile>
        <user-profile>
          <md-card>
            <md-card-header data-background-color="silver">
              <h4 class="title">EDUCATION</h4>
              <p class="category">HyperionDev</p>
            </md-card-header>
            <md-card-content>
              <section class="page-section bg-light" id="education">
                <div class="container">
                  <div class="text-left">
                    <h4>2020</h4>
                    <p>
                      Graduate Student in Software Engineering at HyperionDev
                      school of technology.
                    </p>
                    <h4 class="section-heading text-uppercase">
                      Programming Languages
                    </h4>
                    <nav>
                      <ul>
                        <li class="nav-item">
                          <a class="nav-link" href="#Programming Language"
                            >Java</a
                          >
                        </li>
                        <li class="nav-item">
                          <a class="nav-link" href="#Programming Language"
                            >Python</a
                          >
                        </li>
                        <li class="nav-item">
                          <a class="nav-link" href="#Programming Language"
                            >Javascript</a
                          >
                        </li>
                        <li class="nav-item">
                          <a class="nav-link" href="#Programming Language"
                            >SQL</a
                          >
                        </li>
                      </ul>
                    </nav>
                  </div>
                  <div class="row">
                    <div class="col-lg-4 col-sm-6 mb-4">
                      <!-- Portfolio item 1-->
                      <div class="portfolio-item">
                        <a
                          class="portfolio-link"
                          data-bs-toggle="modal"
                          href="#portfolio"
                        >
                          <div class="portfolio-hover">
                            <div class="portfolio-hover-content">
                              <i class="fas fa-plus fa-3x"></i>
                            </div>
                          </div>
                          <img
                            class="img-fluid"
                            src="assets/img/apple-icon.png"
                            alt="..."
                          />
                        </a>
                        <div class="portfolio-caption">
                          <div class="portfolio-caption-heading">Threads</div>
                          <div class="portfolio-caption-subheading text-muted">
                            Modules
                          </div>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </section>
            </md-card-content>
          </md-card>
        </user-profile>

        <!--About-->
        <md-card>
          <md-card-header data-background-color="silver">
            <h4 class="title">ABOUT</h4>
          </md-card-header>
          <md-card-content>
            <section class="page-section" id="about">
              <div class="container">
                <div class="text-center">
                  <h2 class="section-heading text-uppercase">About</h2>
                  <h3 class="section-subheading text-muted">Info.</h3>
                </div>
                <ul class="timeline">
                  <li>
                    <div class="timeline-image">
                      <img
                        class="rounded-circle img-fluid"
                        src="assets/img/faces/image.jpg"
                        alt="..."
                      />
                    </div>
                    <div class="timeline-panel">
                      <div class="timeline-heading">
                        <h4>2020</h4>
                        <h4 class="subheading">Our Humble Beginnings</h4>
                      </div>
                      <div class="timeline-body">
                        <p class="text-muted">
                          Designed solutions to problems, and express them using
                          pseudo-code and algorithms. Created useful programs in
                          Java and Python, as they are widely used in the tech
                          industry to create mobile applications, web based
                          applications and gaming applications Understood and
                          applied computer science fundamentals, including data
                          structures such as dictionaries, stacks and lists
                          Understood algorithms for sorting and hashing using
                          Big O Notation to analyze the performance of an
                          algorithm Used established algorithms to implement
                          machine learning Used agile development for software
                          development projects Designed, planned, built, tested,
                          debugged, refactored, deployed and maintained a
                          software system Used established design patterns and
                          Git to ensure version control Wrote applications that
                          interact with a database.
                        </p>
                      </div>
                    </div>
                  </li>
                  <li class="timeline-inverted">
                    <div class="timeline-image">
                      <img
                        class="rounded-circle img-fluid"
                        src="assets/img/faces/pc.jpg"
                        alt="..."
                      />
                    </div>
                    <div class="timeline-panel">
                      <div class="timeline-heading">
                        <h4>March 2021</h4>
                        <h4 class="subheading">Journey Started</h4>
                      </div>
                      <div class="timeline-body">
                        <p class="text-muted">
                          Expect in Java, Python and SQL with database analysis
                          and design. Managed to learn Front-end i.e Vue.js and
                          some HTML,CSS.
                        </p>
                      </div>
                    </div>
                  </li>
                  <li>
                    <div class="timeline-image">
                      <img
                        class="rounded-circle img-fluid"
                        src="assets/img/about/3.jpg"
                        alt="..."
                      />
                    </div>
                    <div class="timeline-panel">
                      <div class="timeline-heading">
                        <h4>December 2015</h4>
                        <h4 class="subheading">Transition to Full Service</h4>
                      </div>
                      <div class="timeline-body">
                        Able to now add more skills by learning different
                        languages and frameworks like Springboot Learning more
                        about front-end languages HTML,CSS and Vue.js
                        <p class="text-muted"></p>
                      </div>
                    </div>
                  </li>
                  <li class="timeline-inverted">
                    <div class="timeline-image">
                      <img
                        class="rounded-circle img-fluid"
                        src="assets/img/about/4.jpg"
                        alt="..."
                      />
                    </div>
                    <div class="timeline-panel">
                      <div class="timeline-heading">
                        <h4>July 2020</h4>
                        <h4 class="subheading">Phase Two Expansion</h4>
                      </div>
                      <div class="timeline-body">
                        <p class="text-muted">
                          Building my own applications in Java and also websites
                        </p>
                      </div>
                    </div>
                  </li>
                  <li class="timeline-inverted">
                    <div class="timeline-image">
                      <h4>
                        Be Part
                        <br />
                        Of Our
                        <br />
                        Story!
                      </h4>
                    </div>
                  </li>
                </ul>
              </div>
            </section>
          </md-card-content>
        </md-card>

        <!-- Contact-->
        <md-card>
          <md-card-header data-background-color="silver">
            <h4 class="title">CONTACT</h4>
          </md-card-header>
          <md-card-content>
            <section class="page-section" id="contact">
              <div class="container">
                <div class="text-center">
                  <h2 class="section-heading text-uppercase">Contact Us</h2>
                </div>
                <form id="contactForm" data-sb-form-api-token="API_TOKEN">
                  <div class="row align-items-stretch mb-5">
                    <div class="col-md-6">
                      <div class="form-group">
                        <!-- Name input-->
                        <input
                          class="form-control"
                          id="name"
                          type="text"
                          placeholder="Your Name *"
                          data-sb-validations="required"
                        />
                        <div
                          class="invalid-feedback"
                          data-sb-feedback="name:required"
                        >
                          A name is required.
                        </div>
                      </div>
                      <div class="form-group">
                        <!-- Email address input-->
                        <input
                          class="form-control"
                          id="email"
                          type="email"
                          placeholder="Your Email *"
                          data-sb-validations="required,email"
                        />
                        <div
                          class="invalid-feedback"
                          data-sb-feedback="email:required"
                        >
                          An email is required.
                        </div>
                        <div
                          class="invalid-feedback"
                          data-sb-feedback="email:email"
                        >
                          Email is not valid.
                        </div>
                      </div>
                      <div class="form-group mb-md-0">
                        <!-- Phone number input-->
                        <input
                          class="form-control"
                          id="phone"
                          type="tel"
                          placeholder="Your Phone *"
                          data-sb-validations="required"
                        />
                        <div
                          class="invalid-feedback"
                          data-sb-feedback="phone:required"
                        >
                          A phone number is required.
                        </div>
                      </div>
                    </div>
                    <div class="col-md-6">
                      <div class="form-group form-group-textarea mb-md-0">
                        <!-- Message input-->
                        <textarea
                          class="form-control"
                          id="message"
                          placeholder="Your Message *"
                          data-sb-validations="required"
                        ></textarea>
                        <div
                          class="invalid-feedback"
                          data-sb-feedback="message:required"
                        >
                          A message is required.
                        </div>
                      </div>
                    </div>
                  </div>
                  <div class="d-none" id="submitSuccessMessage">
                    <div class="text-center text-white mb-3">
                      <div class="fw-bolder"></div>
                      <br />
                      <a
                        href="https://startbootstrap.com/solution/contact-forms"
                      ></a>
                    </div>
                  </div>
                  <!-- Submit error message-->
                  <!---->
                  <!-- This is what your users will see when there is-->
                  <!-- an error submitting the form-->
                  <div class="d-none" id="submitErrorMessage">
                    <div class="text-center text-danger mb-3"></div>
                  </div>
                  <!-- Submit Button-->
                  <div class="text-center">
                    <button
                      class="btn btn-primary btn-xl text-uppercase disabled"
                      id="submitButton"
                      type="submit"
                    >
                      Send Message
                    </button>
                  </div>
                </form>
              </div>
            </section>
          </md-card-content>
        </md-card>
        <!--profile-->
        <div class="col-sm-4">
          <div class="text-center">
            <h6>follow us</h6>
            <md-button
              class="md-sm md-just-icon"
              href="https://github.com/garikai94/profile_app"
              ><i class="fab fa-github"></i
            ></md-button>
            <md-button class="md-sm md-just-icon" href="#!"
              ><i class="fab fa-twitter"></i
            ></md-button>
            <md-button class="md-sm md-just-icon" href="https://www.facebook.com/public/Tafadzwa-G-Matanhatu"
              ><i class="fab fa-facebook f"></i
            ></md-button>
            <md-button
              class="md-sm md-just-icon"
              href="https://za.linkedin.com/garikai-matanhatu"
              ><i class="fab fa-linkedin-in"></i
            ></md-button>
          </div>
        </div>
        ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
      </div>
    </div>
  </div>
</template>
<script>
import { EditProfileForm, UserCard } from "@/pages";
export default {
  components: {
    EditProfileForm,
    UserCard,
  },
};
</script>
