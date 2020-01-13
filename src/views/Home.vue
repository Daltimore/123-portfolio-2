<template>
  <main id="first-theme">
    <div class="row">
      <div class="col-lg-12 col-md-12 d-flex justify-space-between m-0 p-0">
        <div class="col-lg-6 col-md-6 col-sm-12">
          <div class="avatar-section">
            <div class="row">
              <div class="col-lg-3 avatar">
                <img src="@/assets/img/avatar.png" alt="">
              </div>
              <div class="col-lg-6 user-details">
                <h4>Conor</h4>
                <p>Ui/Ux designer</p>
                <div class="d-flex justify-content-between">
                  <div class="rate">
                    <span>&#x24;10</span>
                    <p>Hourly Rate</p>
                  </div>
                  <div class="rate">
                    <span>35 hours</span>
                    <p>Weekly Availability</p>
                  </div>
                </div>
              </div>
              <div class="col-lg-3 audio-section">
                <div class="interv__container">
                  <p>interviews</p>
                  <div class="interv">
                    <span>
                      <img src="@/assets/img/sound.svg" alt="">
                    </span>
                    <span>
                      <img src="@/assets/img/video-player.svg" alt="">
                    </span>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div>
            <div class="row tap-section">
              <div class="col-lg-6">
                <button class="btn btn-sm">Tap to chat</button>
              </div>
              <div class="col-lg-6 icon-container">
                <div>
                  <i class="fab fa-behance"></i>
                </div>
                <div>
                  <i class="fab fa-dribbble"></i>
                </div>
                <div>
                  <i class="fab fa-instagram"></i>
                </div>
                <div>
                  <i class="fab fa-linkedin-in"></i>
                </div>
                <div>
                  <img src="@/assets/img/google.png" alt="">
                </div>
              </div>
            </div>
          </div>
          <div class="d-flex justify-content-center align-item-center hire-me">
              <button class="btn btn-md">Hire me</button>
            </div>

            <section class="portfolio-section">
              <tab-component></tab-component>
            </section>
        </div>
        <div class="col-lg-6 col-md-6 col-sm-12 purple-section">
          <div class="col-lg-1 line">
            <div class="straight-line"></div>
          </div>
          <div class="col-lg-11">
            <section class="work__section">
              <div id="tabs" class="tab__section">
                <div>
                  <img src="@/assets/img/left-arrow.svg" alt="" class="pr-3 move-left">
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
                  @click.prevent="setActive('work', 1)">

                  <h5 :class="{ active: isActive('work') }">Work</h5>
                </a>
              </div>
              <div>
                <a 
                  id="third-tab"
                  data-toggle="tab"
                  role="tab"
                  aria-controls="third"
                  aria-selected="true"
                  @click.prevent="setActive('education', 2)">

                  <h5 :class="{ active: isActive('education') }">Education</h5>
                </a>
              </div>
              <div @click="moveRight">
                <img src="@/assets/img/right-arrow.svg" alt="" class="pr-3 move-right">
              </div>
              </div>

              <div id="myTabContent" class="tab-content">
                <div
                  id="portfolio"
                  class="tab-pane"
                  role="tabpanel"
                  aria-labelledby="first-tab"
                  :class="{ 'active show': isActive('portfolio') }">

                  <div class="img-section">
                    <div class="col-lg-6 col-md-12 col-sm-12">
                      <img src="@/assets/img/image1.png" alt="">
                    </div>
                    <div class="col-lg-6 col-md-12 col-sm-12 mask">
                      <img src="@/assets/img/image2.png" alt="">
                    </div>
                  </div>
                </div>

                <div
                  id="work"
                  class="tab-pane"
                  role="tabpanel"
                  aria-labelledby="second-tab"
                  :class="{ 'active show': isActive('work') }">

                  <div class="work-details">
                    <div class="work-details__head">
                      <div class="work-content">
                        <div class="pl-4">
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
                        <div class="pl-4">
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
                        <div class="pl-4">
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
                  aria-labelledby="third-tab"
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
      </div>
    </div>
  </main>
</template>

<script>
import TabComponent from '@/components/TabComponent'

export default {
  components: {
    TabComponent
  },
  data() {
    return {
      activeItem: 'portfolio',
      currentLink: null,
      current: null
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