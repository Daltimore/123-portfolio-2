<template>
  <div id="social-tabs-mobile">
    <vue-tabs>
      <v-tab title="Programming Languages">
        <div class="d-flex justify-content-between align-items-center">
          <div class="ai">
            <span>Ai</span>
          </div>
          <div class="ps">
            <span>Ps</span>
          </div>
          <i class="fab fa-sketch fa-2x diamond"></i>
          <div class="ui">
          <span>Ui</span>
        </div>
        <div class="ux">
          <span>Ux</span>
        </div>
        </div>
      </v-tab>

      <v-tab title="Frameworks/Databases">
        Second tab content
      </v-tab>

      <v-tab title="Digital skills">
        Third tab content
      </v-tab>

      <v-tab title="Software">
        Fourth tab content
      </v-tab>
    </vue-tabs>
  </div>
</template>

<script>

export default {

}
</script>

<style>
#social-tabs-mobile .vue-tabs .nav > li span.title {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  font-size: 12px !important;
}

#social-tabs-mobile .vue-tabs .nav-tabs > li.active > a, .vue-tabs .nav-tabs > li.active > a:hover, .vue-tabs .nav-tabs > li.active > a:focus {
  color: #ffffff;
  background: transparent;
  border-bottom: 2px solid #ffffff !important; 
  border: none;
  cursor: default;
}

#social-tabs-mobile .vue-tabs .nav-tabs {
  border-bottom: 1px solid #4D75E8;
}

#social-tabs-mobile .vue-tabs .tabs__link {
  color: #ffffff;
  opacity: 0.6;
}

#social-tabs-mobile .vue-tabs .tabs__link:active {
  color: #ffffff;
}

#social-tabs-mobile .vue-tabs .nav {
  margin-bottom: 0;
  margin-top: 0;
  padding-left: 40px;
  list-style: none;
  width: 95%;
}

#social-tabs-mobile .tab-content {
  padding-top: 3rem;
  padding-left: 10rem;
  padding-right: 10rem;
}

#social-tabs-mobile .ai {
  width: 2rem;
  height: 2rem;
  padding: 0.5rem;
  border-radius: 100%;
  display: flex;
  align-items: center;
  background: #5E3C16;
  color: #DF871E;
}

#social-tabs-mobile .ps {
  width: 2rem;
  height: 2rem;
  padding: 0.5rem;
  border-radius: 100%;
  display: flex;
  align-items: center;
  background: #2A4997;
  color: #76C8DA;
}

#social-tabs-mobile .diamond {
  color: #FFCA28;
}

#social-tabs-mobile .ui {
  background: #ffffff;
  width: 2rem;
  height: 2rem;
  padding: 0.5rem;
  border-radius: 100%;
  display: flex;
  align-items: center;
  color: #4D75E8;
}

#social-tabs-mobile .ux {
  background: #ffffff;
  width: 2rem;
  height: 2rem;
  padding: 0.47rem;
  border-radius: 100%;
  display: flex;
  align-items: center;
  color: #4D75E8;
}
</style>
