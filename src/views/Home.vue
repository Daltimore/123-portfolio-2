<template>
  <main id="home">
    <div class="col-12 main-container">
      <div class="col-4 user-details-container">
        <div class="d-flex justify-content-between user-deets">
          <img src="@/assets/img/avatar.png" alt="" class="avatar">
            <div class="user-details">
              <h5>Conor</h5>
              <p>Ui/Ux designer</p>
            </div>
        </div>
        <div class="d-flex justify-content-between">
          <div class="button-container">
            <a href="#" class="tap-to-chat">
              <img src="@/assets/img/chat.svg" alt="" class="chat">
              <span class="text">
                Tap to chat
              </span>
            </a>
          </div>
          <div class="icon-container">
            <div class="icon">
              <i class="fab fa-behance"></i>
            </div>
            <div class="icon">
              <i class="fab fa-dribbble"></i>
            </div>
            <div class="icon">
              <i class="fab fa-instagram"></i>
            </div>
            <div class="icon">
              <i class="fab fa-linkedin-in"></i>
            </div>
            <div class="icon">
              <img src="@/assets/img/google.svg" alt="">
            </div>
          </div>
        </div>
      </div>
      <div class="col-12 user-deets__mobile">
        <div class="mobile-main__container">
          <div class="d-flex">
          <img src="@/assets/img/avatar.png" alt="" class="avatar">
          <div class="user-details">
            <h5>Conor</h5>
            <p>Ui/Ux designer</p>
            <div class="user__rate">
              <div>
              <span>$10</span>
              <p>Hourly rate</p>
            </div>
            <div class="rate">
              <span>35 hours</span>
              <p>Weekly Availability</p>
            </div>
            </div>
          </div>
        </div>
        <div class="mobile-interview__container">
          <p>Interview:</p>
          <div class="mobile_image">
            <span>
              <img src="@/assets/img/sound.svg" alt="">
            </span>
            <span>
              <img src="@/assets/img/video-player.svg" alt="">
            </span>
          </div>
        </div>
        </div>
        <div class="mobile-social__section">
          <div class="tab__mobile">
            <button>Tap to chat</button>
          </div>
          <div class="mobile-icon__cont">
            <div class="icon">
              <i class="fab fa-behance"></i>
            </div>
            <div class="icon">
              <i class="fab fa-dribbble"></i>
            </div>
            <div class="icon">
              <i class="fab fa-instagram"></i>
            </div>
            <div class="icon">
              <i class="fab fa-linkedin-in"></i>
            </div>
            <div class="icon">
              <img src="@/assets/img/google.svg" alt="">
            </div>
          </div>
        </div>
        <div class="d-flex justify-content-center align-items-center pt-5">
          <button class="hire">Hire me</button>
        </div>
      </div>
      <div class="col-5 availability-container">
        <div class="d-flex">
          <p class="availability-p">Interview: </p>
          <div class="audio__container">
            <span class="purple-area">
              <img src="@/assets/img/video-player.svg" alt="">
            </span>
            <span class="purple-area">
              <img src="@/assets/img/sound.svg" alt="">
            </span>
          </div>
        </div>
        <div class="d-flex justify-content-between action-area">
          <div>
            <span>&#x24;10</span>
            <p>Hourly Rate</p>
          </div>
          <div>
            <span>35 hours</span>
             <p>Weekly Availability</p>
          </div>
          <div>
            <button>Hire me</button>
          </div>
        </div>
      </div>
    </div>
    <div class="tab-containerr">
      <div>
        <img src="@/assets/img/left.svg" alt="">
      </div>
      <div>
          <a 
            id="first-tab"
            :class="{ active: isActive('portfolio') }"
            data-toggle="tab"
            role="tab"
            aria-controls="first"
            aria-selected="true"
            @click.prevent="setActive('portfolio', 0)">
            
            <h5 :class="{ active: isActive('portfolio') }">Portfolio</h5>
          </a>
      </div>
      <div>
        <a 
          id="second-tab"
          data-toggle="tab"
          role="tab"
          aria-controls="second"
          aria-selected="true"
          @click.prevent="setActive('skills', 1)">

          <h5 :class="{ active: isActive('skills') }">Skills</h5>
        </a>
      </div>
      <div>
          <a 
            id="third-tab"
            data-toggle="tab"
            role="tab"
            aria-controls="third"
            aria-selected="true"
            @click.prevent="setActive('work', 2)">

            <h5 :class="{ active: isActive('work') }">Work</h5>
          </a>
        </div>
        <div>
          <a 
            id="fourth-tab"
            data-toggle="tab"
            role="tab"
            aria-controls="fourth"
            aria-selected="true"
            @click.prevent="setActive('education', 3)">

            <h5 :class="{ active: isActive('education') }">Education</h5>
          </a>
        </div>
      <div>
        <img src="@/assets/img/right.svg" alt="">
      </div>
    </div>

    <section class="tab-section">
      <div class="col-lg-12 col-md-12 col-sm-12 purple-section">
        <div class="col-lg-11">
          <section class="work__section">
            <div id="myTabContent" class="tab-content">
              <div
                id="portfolio"
                class="tab-pane"
                role="tabpanel"
                aria-labelledby="first-tab"
                :class="{ 'active show': isActive('portfolio') }">

                <div class="img-section">
                  <div class="col-lg-6 col-md-12 col-sm-12">
                    <img src="@/assets/img/phone.png" alt="">
                  </div>
                  <div class="col-lg-6 col-md-12 col-sm-12 mask">
                    <img src="@/assets/img/hulk.png" alt="">
                  </div>
                </div>
              </div>

              <div
                id="portfolio"
                class="tab-pane"
                role="tabpanel"
                aria-labelledby="second-tab"
                :class="{ 'active show': isActive('skills') }">
                <div class="mobile__tab">
                  <mobile-tab-component></mobile-tab-component>
                </div>
              </div>

              <div
                id="work"
                class="tab-pane"
                role="tabpanel"
                aria-labelledby="third-tab"
                :class="{ 'active show': isActive('work') }">

                <div class="work-details">
                  <div class="work-details__head">
                    <div class="work-content">
                      <div class="pl-4 mobile">
                        <h6>Graphic&amp;<br />Web Designer</h6>
                        <p class="pt-5">2018 - 2019</p>
                      </div>
                    <div class="">
                        <h6 class="sub-heading">Company "React"</h6>
                        <ul class="list-unstyled">
                          <li>
                            - Turning creative concepts into finished websites.
                          </li>
                          <li>
                            - Drawing up detailed website s pecifications.
                          </li>
                          <li>
                            - Building websites that are easy to understand, navigate and use.
                          </li>
                          <li>
                            - Designing sample page layouts.
                          </li>
                          <li>
                            - Ensuring that the website complies with the company’s brand guidelines.
                          </li>
                        </ul>
                      </div>
                    </div>
                  </div>
                    <div class="work-details__head">
                    <div class="work-content">
                      <div class="pl-4 mobile">
                        <h6>Graphic&amp;<br />Web Designer</h6>
                        <p class="pt-5">2018 - 2019</p>
                      </div>
                    <div>
                        <h6 class="sub-heading">Company "React"</h6>
                        <ul class="list-unstyled">
                          <li>
                            - Turning creative concepts into finished websites.
                          </li>
                          <li>
                            - Drawing up detailed website s pecifications.
                          </li>
                          <li>
                            - Building websites that are easy to understand, navigate and use.
                          </li>
                          <li>
                            - Designing sample page layouts.
                          </li>
                          <li>
                            - Ensuring that the website complies with the company’s brand guidelines.
                          </li>
                        </ul>
                      </div>
                    </div>
                  </div>
                  <div class="work-details__head">
                    <div class="work-content">
                      <div class="pl-4 mobile">
                        <h6>Graphic&amp;<br />Web Designer</h6>
                        <p class="pt-5">2018 - 2019</p>
                      </div>
                    <div>
                        <h6 class="sub-heading">Company "React"</h6>
                        <ul class="list-unstyled">
                          <li>
                            - Turning creative concepts into finished websites.
                          </li>
                          <li>
                            - Drawing up detailed website s pecifications.
                          </li>
                          <li>
                            - Building websites that are easy to understand, navigate and use.
                          </li>
                          <li>
                            - Designing sample page layouts.
                          </li>
                          <li>
                            - Ensuring that the website complies with the company’s brand guidelines.
                          </li>
                        </ul>
                      </div>
                    </div>
                  </div>
                </div>
              </div>

              <div
                id="education"
                class="tab-pane"
                role="tabpanel"
                aria-labelledby="fourth-tab"
                :class="{ 'active show': isActive('education') }">

                <div class="work-details">
                  <div class="work-details__head">
                    <div class="work-content">
                    <div  class="pl-4">
                      <h6>Master in <br />Web Developer</h6>
                      <p class="pt-3">2015 - 2016</p>
                    </div>
                      <div>
                        <p>Envision Media, Inc., Santa Cruz, CA </p>
                    </div>
                    </div>
                  </div>
                  

                  <div class="work-details__head">
                    <div class="work-content">
                    <div  class="pl-4">
                      <h6>Master in <br />Web Developer</h6>
                      <p class="pt-3">2018 - 2019</p>
                    </div>
                      <div>
                        <p>Massachusetts Institute of Technology (MIT) Boston, MA </p>
                    </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </section>
        </div>
        <div class="col-lg-1 line">
          <div class="straight-line"></div>
        </div>
      </div>
    </section>

    <section class="tab-section__mobile">
      <div class="tab-containerr__mobile">
      <div class="left">
        <img src="@/assets/img/left-mobile.svg" alt="">
      </div>
      <div>
          <a 
            id="first-tab"
            :class="{ active: isActive('portfolio') }"
            data-toggle="tab"
            role="tab"
            aria-controls="first"
            aria-selected="true"
            @click.prevent="setActive('portfolio', 0)">
            
            <h5 :class="{ active: isActive('portfolio') }">Portfolio</h5>
          </a>
      </div>
      <div>
        <a 
          id="second-tab"
          data-toggle="tab"
          role="tab"
          aria-controls="second"
          aria-selected="true"
          @click.prevent="setActive('skills', 1)">

          <h5 :class="{ active: isActive('skills') }">Skills</h5>
        </a>
      </div>
      <div>
          <a 
            id="third-tab"
            data-toggle="tab"
            role="tab"
            aria-controls="third"
            aria-selected="true"
            @click.prevent="setActive('work', 2)">

            <h5 :class="{ active: isActive('work') }">Work</h5>
          </a>
        </div>
        <div>
          <a 
            id="fourth-tab"
            data-toggle="tab"
            role="tab"
            aria-controls="fourth"
            aria-selected="true"
            @click.prevent="setActive('education', 3)">

            <h5 :class="{ active: isActive('education') }">Education</h5>
          </a>
        </div>
      <div class="right">
        <img src="@/assets/img/right-mobile.svg" alt="">
      </div>
    </div>
      <div class="col-lg-12 col-md-12 col-sm-12 purple-section">
        <div class="col-lg-11">
          <section class="work__section">
            <div id="myTabContent" class="tab-content">
              <div
                id="portfolio"
                class="tab-pane"
                role="tabpanel"
                aria-labelledby="first-tab"
                :class="{ 'active show': isActive('portfolio') }">

                <div class="img-section">
                  <div class="col-lg-6 col-md-12 col-sm-12">
                    <img src="@/assets/img/phone.png" alt="">
                  </div>
                  <div class="col-lg-6 col-md-12 col-sm-12 mask">
                    <img src="@/assets/img/hulk.png" alt="">
                  </div>
                </div>
              </div>

              <div
                id="portfolio"
                class="tab-pane"
                role="tabpanel"
                aria-labelledby="second-tab"
                :class="{ 'active show': isActive('skills') }">
                <div class="mobile__tab">
                  <tab-component></tab-component>
                </div>
              </div>

              <div
                id="work"
                class="tab-pane"
                role="tabpanel"
                aria-labelledby="third-tab"
                :class="{ 'active show': isActive('work') }">

                <div class="work-details">
                  <div class="work-details__head">
                    <div class="work-content">
                      <div class="pl-4 mobile">
                        <h6>Graphic&amp;<br />Web Designer</h6>
                        <p class="pt-5">2018 - 2019</p>
                      </div>
                    <div class="">
                        <h6 class="sub-heading">Company "React"</h6>
                        <ul class="list-unstyled">
                          <li>
                            - Turning creative concepts into finished websites.
                          </li>
                          <li>
                            - Drawing up detailed website s pecifications.
                          </li>
                          <li>
                            - Building websites that are easy to understand, navigate and use.
                          </li>
                          <li>
                            - Designing sample page layouts.
                          </li>
                          <li>
                            - Ensuring that the website complies with the company’s brand guidelines.
                          </li>
                        </ul>
                      </div>
                    </div>
                  </div>
                    <div class="work-details__head">
                    <div class="work-content">
                      <div class="pl-4 mobile">
                        <h6>Graphic&amp;<br />Web Designer</h6>
                        <p class="pt-5">2018 - 2019</p>
                      </div>
                    <div>
                        <h6 class="sub-heading">Company "React"</h6>
                        <ul class="list-unstyled">
                          <li>
                            - Turning creative concepts into finished websites.
                          </li>
                          <li>
                            - Drawing up detailed website s pecifications.
                          </li>
                          <li>
                            - Building websites that are easy to understand, navigate and use.
                          </li>
                          <li>
                            - Designing sample page layouts.
                          </li>
                          <li>
                            - Ensuring that the website complies with the company’s brand guidelines.
                          </li>
                        </ul>
                      </div>
                    </div>
                  </div>
                  <div class="work-details__head">
                    <div class="work-content">
                      <div class="pl-4 mobile">
                        <h6>Graphic&amp;<br />Web Designer</h6>
                        <p class="pt-5">2018 - 2019</p>
                      </div>
                    <div>
                        <h6 class="sub-heading">Company "React"</h6>
                        <ul class="list-unstyled">
                          <li>
                            - Turning creative concepts into finished websites.
                          </li>
                          <li>
                            - Drawing up detailed website s pecifications.
                          </li>
                          <li>
                            - Building websites that are easy to understand, navigate and use.
                          </li>
                          <li>
                            - Designing sample page layouts.
                          </li>
                          <li>
                            - Ensuring that the website complies with the company’s brand guidelines.
                          </li>
                        </ul>
                      </div>
                    </div>
                  </div>
                </div>
              </div>

              <div
                id="education"
                class="tab-pane"
                role="tabpanel"
                aria-labelledby="fourth-tab"
                :class="{ 'active show': isActive('education') }">

                <div class="work-details">
                  <div class="work-details__head">
                    <div class="work-content">
                    <div  class="pl-4">
                      <h6>Master in <br />Web Developer</h6>
                      <p class="pt-3">2015 - 2016</p>
                    </div>
                      <div>
                        <p>Envision Media, Inc., Santa Cruz, CA </p>
                    </div>
                    </div>
                  </div>
                  

                  <div class="work-details__head">
                    <div class="work-content">
                    <div  class="pl-4">
                      <h6>Master in <br />Web Developer</h6>
                      <p class="pt-3">2018 - 2019</p>
                    </div>
                      <div>
                        <p>Massachusetts Institute of Technology (MIT) Boston, MA </p>
                    </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </section>
        </div>
      </div>
    </section>
  </main>
</template>

<script>
import MobileTabComponent from '@/components/MobileTabComponent.vue';
import TabComponent from '@/components/TabComponent.vue'

export default {
  components: {
    MobileTabComponent,
    TabComponent
  },
  data() {
    return {
      activeItem: 'portfolio',
      currentLink: null
    }
  },
  methods: {
    isActive (menuItem) {
      return this.activeItem === menuItem;
    },
   setActive (menuItem, y) {
      this.activeItem = menuItem;
      this.currentLink = y
    },
    moveRight() {
      this.current++;
    },
    moveLeft() {
      this.current--;
    }
  }
}
</script>

<style scoped>

</style>