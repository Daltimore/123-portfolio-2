<template>
  <div class="">
    <vue-tabs>
      <v-tab title="Programming Languages">
        <div class="d-flex justify-content-between align-items-center">
          <div class="ai">
            <span>Ai</span>
          </div>
          <div class="ps">
            <span>Ps</span>
          </div>
          <i class="fab fa-sketch fa-2x"></i>
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
.vue-tabs .nav > li span.title {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  font-size: 12px !important;
}

.vue-tabs .nav-tabs > li.active > a, .vue-tabs .nav-tabs > li.active > a:hover, .vue-tabs .nav-tabs > li.active > a:focus {
  color: #555555;
  background-color: #fff;
  border-bottom: 2px solid #4D75E8 !important; 
  border: none;
  cursor: default;
}

.vue-tabs .nav {
  margin-bottom: 0;
  margin-top: 0;
  padding-left: 40px;
  list-style: none;
  width: 87%;
}

.tab-content {
  padding: 2rem 4rem;
}

.ai {
  width: 2rem;
  height: 2rem;
  padding: 0.5rem;
  border-radius: 100%;
  display: flex;
  align-items: center;
  background: #5E3C16;
  color: #DF871E;
}

.ps {
  width: 2rem;
  height: 2rem;
  padding: 0.5rem;
  border-radius: 100%;
  display: flex;
  align-items: center;
  background: #2A4997;
  color: #76C8DA;
}

.ui {
  background: #4D75E8;
  width: 2rem;
  height: 2rem;
  padding: 0.5rem;
  border-radius: 100%;
  display: flex;
  align-items: center;
  color: #ffffff;
}

.ux {
  background: #4D75E8;
  width: 2rem;
  height: 2rem;
  padding: 0.47rem;
  border-radius: 100%;
  display: flex;
  align-items: center;
  color: #ffffff;
}
</style>
