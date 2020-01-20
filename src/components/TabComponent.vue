<template>
  <div id="social-tabs">
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
        
      </v-tab>

      <v-tab title="Digital skills">
        
      </v-tab>

      <v-tab title="Software">
        
      </v-tab>
    </vue-tabs>
  </div>
</template>

<script>

export default {

}
</script>

<style>
#social-tabs .vue-tabs .nav > li span.title {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  font-size: 12px !important;
}

#social-tabs .vue-tabs .nav-tabs > li.active > a, .vue-tabs .nav-tabs > li.active > a:hover, .vue-tabs .nav-tabs > li.active > a:focus {
  color: #ffffff !important;
  background-color: transparent;
  border-bottom: 2px solid #ffffff !important; 
  border: none;
  cursor: default;
}

#social-tabs .vue-tabs .nav {
  margin-bottom: 0;
  margin-top: 0;
  padding-left: 40px;
  list-style: none;
  width: 100%;
}

#social-tabs .tab-content {
  padding-top: 3rem;
  padding-left: 10rem;
  padding-right: 10rem;
}

#social-tabs .ai {
  width: 2rem;
  height: 2rem;
  padding: 0.5rem;
  border-radius: 100%;
  display: flex;
  align-items: center;
  background: #5E3C16;
  color: #DF871E;
}

#social-tabs .ps {
  width: 2rem;
  height: 2rem;
  padding: 0.5rem;
  border-radius: 100%;
  display: flex;
  align-items: center;
  background: #2A4997;
  color: #76C8DA;
}

#social-tabs .diamond {
  color: #FFCA28;
}

#social-tabs .ui {
  background: #4D75E8;
  width: 2rem;
  height: 2rem;
  padding: 0.5rem;
  border-radius: 100%;
  display: flex;
  align-items: center;
  color: #ffffff;
}

#social-tabs .ux {
  background: #4D75E8;
  width: 2rem;
  height: 2rem;
  padding: 0.47rem;
  border-radius: 100%;
  display: flex;
  align-items: center;
  color: #ffffff;
}

.vue-tabs .tabs__link {
    color: #ffffff;
    opacity: 0.6;
  }

  @media (min-width: 320px) and (max-width: 370px) {
    #social-tabs .tab-content {
    padding-top: 3rem;
    padding-left: 1rem !important;
    padding-right: 1rem !important;
  }
}
</style>
