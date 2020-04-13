<template>
  <v-app>
    <v-container>
      <v-card flat>
        <div class="text-center mt-12">
          <v-avatar size="200" class="mt-5">
            <img src="../assets/Liben.jpg" alt="Liben's Picture" />
          </v-avatar>
        </div>

        <v-tabs
          v-model="tab"
          background-color="transparent"
          grow
          class="pt-lg-12 pb-lg-12 pt-md-8 pb-md-8 pt-lg-5 pb-lg-5"
        >
          <v-tab v-for="item in items" :key="item">{{ item }}</v-tab>

          <v-tab-item class="mt-lg-8 mt-md-6 mt-sm-6">
            <p>{{text}}</p>
          </v-tab-item>

          <v-tab-item class="mt-lg-8 mt-md-6 mt-sm-6">
            <div class="text-center">
              <p class="headline">a lot more coming...</p>
            </div>

            <v-row>
              <v-card class="mx-auto" max-width="344" outlined>
                <v-list-item three-line>
                  <v-list-item-content>
                    <v-list-item-title class="headline mb-1">Flutter Quiz App</v-list-item-title>
                    <v-list-item-subtitle>a quiz app that asks quiz based on the category selected.</v-list-item-subtitle>
                  </v-list-item-content>

                  <v-list-item-avatar tile size="80">
                    <v-img src="../assets/general.png"></v-img>
                  </v-list-item-avatar>
                </v-list-item>

                <v-card-actions>
                  <a href="https://github.com/LibenHailu/quiz_app" target="_blank">
                    <img src="https://img.icons8.com/windows/50/000000/github.png" />
                  </a>
                  <a href="https://youtu.be/vOE5l30lkac" target="_blank">
                    <img src="https://img.icons8.com/ios/50/000000/youtube.png" />
                  </a>
                </v-card-actions>
              </v-card>

              <v-card class="mx-auto mt-6" max-width="344" outlined>
                <v-list-item three-line>
                  <v-list-item-content>
                    <v-list-item-title class="headline mb-1">Javascript Weather App</v-list-item-title>
                    <v-list-item-subtitle>a weather app that provides weather info for the asked city.</v-list-item-subtitle>
                  </v-list-item-content>

                  <v-list-item-avatar tile size="80">
                    <v-img src="../assets/weather.png"></v-img>
                  </v-list-item-avatar>
                </v-list-item>

                <v-card-actions>
                  <a href="https://github.com/LibenHailu/weather-website" target="_blank">
                    <img src="https://img.icons8.com/windows/50/000000/github.png" />
                  </a>
                  <a
                    href="https://liben-weather-application.herokuapp.com/"
                    target="_blank"
                  >Website link</a>
                </v-card-actions>
              </v-card>

              <v-card class="mx-auto mt-6" max-width="344" outlined>
                <v-list-item three-line>
                  <v-list-item-content>
                    <v-list-item-title class="headline mb-1">Vue Quiz App</v-list-item-title>
                    <v-list-item-subtitle>
                      developed for the hackathon
                      <a
                        href="https://ethio-hacks-7th-series.devpost.com/?ref_content=default&ref_feature=challenge&ref_medium=portfolio"
                        target="_blank"
                      >here</a> by me and my friends.
                    </v-list-item-subtitle>
                  </v-list-item-content>

                  <v-list-item-avatar tile size="80">
                    <v-img src="../assets/quiz.png"></v-img>
                  </v-list-item-avatar>
                </v-list-item>

                <v-card-actions>
                  <a href="https://github.com/LibenHailu/quiz-app-vue" target="_blank">
                    <img src="https://img.icons8.com/windows/50/000000/github.png" />
                  </a>
                  <a href="https://quiz-app-vue-2ec58.web.app/" target="_blank">Website link</a>
                </v-card-actions>
              </v-card>
            </v-row>
          </v-tab-item>

          <v-tab-item class="mt-lg-12 mt-md-6 mt-sm-6 ">
            <v-row justify="space-around">
              <a href="https://www.facebook.com/liben.haylu" target="_blank">
                <img
                  src="https://img.icons8.com/color/50/000000/facebook-new.png"
                  alt="facebook link"
                />
              </a>
              <a href="https://twitter.com/HailuLiben">
                <img src="https://img.icons8.com/color/50/000000/twitter.png" alt="twitter link" />
              </a>
              <a href="https://github.com/LibenHailu">
                <img src="https://img.icons8.com/windows/50/000000/github.png" alt="github link" />
              </a>
            </v-row>
          </v-tab-item>
        </v-tabs>
      </v-card>
    </v-container>
  </v-app>
</template>

<style>
a {
  text-decoration: none;
}
p {
  font-size: 18px;
}
</style>


<script>
export default {
  data() {
    return {
      tab: null,
      items: ["About", "Portfolio", "Contact"],
      text:
        "Hello, I'm Liben Hailu. I am a Frontend Developer. I have experience over 4 years in programming. and I have a good experience in developing a wide range of systems using popular languages. I am currently focused on frontend specially vue.js and mobile apps with flutter. and something you may not know about me is I have a curious mind."
    };
  }
};
</script>