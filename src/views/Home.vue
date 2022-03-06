<template>
  <div id="home">
    <v-navigation-drawer
      v-model="drawer"
      fixed
    >
      <v-list
        nav
        dense
      >
        <v-list-item-group
        >
          <v-list-item disabled>
            <v-list-item-title>
              <span class="text-h5">
                楊婷婷 Raquel Yang
              </span>
            </v-list-item-title>
          </v-list-item>
          <v-divider class="my-5"></v-divider>
          <v-list-item href="#home" >
            <v-list-item-title>
              <span class="text-subtitle-1">個人簡介</span>
            </v-list-item-title>
          </v-list-item>

          <v-list-item href="#educationandexperience" >
            <v-list-item-title>
              <span class="text-subtitle-1">學經歷</span>
            </v-list-item-title>
          </v-list-item>

          <v-list-item href="#skill" >
            <v-list-item-title>
              <span class="text-subtitle-1">技能</span>
            </v-list-item-title>
          </v-list-item>

          <v-list-item href="#portfolio" >
            <v-list-item-title>
              <span class="text-subtitle-1">作品集</span>
            </v-list-item-title>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>
      <v-app-bar
      class="nav"
      fixed
      flat
      >
        <v-container class="name">
          <v-row class="nav">
            <a href="#">
              <h1 class="text-h5">楊婷婷<span class="text-h6 ml-4">Raquel Yang</span></h1>
            </a>
            <v-spacer></v-spacer>
            <a href="#home" v-smooth-scroll="{offset: -100}" class="hidden-sm-and-down">個人簡介</a>
            <a href="#educationandexperience" v-smooth-scroll="{offset: -100}" class="hidden-sm-and-down">學經歷</a>
            <a href="#skill" v-smooth-scroll="{offset: -100}" class="hidden-sm-and-down">技能</a>
            <a href="#portfolio" v-smooth-scroll="{offset: -100}" class="hidden-sm-and-down">作品集</a>
            <v-app-bar-nav-icon @click="drawer=!drawer" class="hidden-md-and-up"></v-app-bar-nav-icon>
          </v-row>

        </v-container>
      </v-app-bar>
    <!-- top -->
    <v-container class="maincontent px-5 py-5">
      <v-row>
        <v-col cols="12" sm="6" md="4">
          <v-row class="justify-center">
            <v-col cols="12">
              <v-img src="../assets/images/self.jpeg" class="rounded px-16 py-16"></v-img>
            </v-col>
            <v-col cols="12">
              <!-- <h1 class="text-h5">楊婷婷<span class="text-h5 ml-4">Raquel Yang</span></h1> -->
              <!-- <div class="mt-5 d-flex align-center">
                <v-icon left large>mdi-school</v-icon>
                <span class="text-h6">臺北科技大學/材料所 <span class="grey--text text--darken-2 text-subtitle-1">2015 - 2017</span></span>
              </div>
              <div class="mt-5 d-flex align-center">
                <v-icon left large>mdi-school</v-icon>
                <span class="text-h6">臺北科技大學/材料與資源工程學系 <span class="grey--text text--darken-2 text-subtitle-1">2010 - 2015</span></span>
              </div> -->
              <div>
                <v-icon left>mdi-email-outline</v-icon>
                <a href="mailto:lorehmmoreh007@gmail.com">
                  <span>lorehmmoreh007@gmail.com</span>
                </a>
              </div>
              <div class="mt-2">
                <v-icon left>mdi-github</v-icon>
                <a href="https://github.com/RaquelYang">
                  <span>https://github.com/RaquelYang</span>
                </a>
              </div>
            </v-col>
          </v-row>
        </v-col>
        <v-col cols="12" sm="6" md="8">
          <v-col cols="12" class="text-h4">個人簡介</v-col>
        <v-col cols="12" class="portfolio">
          <p>
            我畢業於臺北科技大學材料所，在研究過程接觸到程式相關的應用技術，於是對程式設計產生興趣。在工作期間思考著未來轉型的方向，於是決定開啟轉職前端工程師的道路。
          </p>
          <p>
            透過半年的前端網頁開發技術課程，熟悉HTML、CSS、JavaScript 及 Vue.js 進行網頁的開發，可使用 Node.js 及 MongoDB 建置後端資料庫，並且部署在 heroku 完成前後端網頁整合。
          </p>
          <p>
            未來期許在轉職道路上能夠持續精進，研究各種前端新技術，用於公司的專案及產品的開發，成為一位可以解決問題的工程師。
          </p>
        </v-col>
        </v-col>

      </v-row>
      <!-- 個人簡介 -->
    <!-- 經歷 -->
    <v-row id="educationandexperience">
      <v-col cols="12" md="6">
        <p class="text-h4 my-10">學歷</p>
        <v-timeline
          dense
          clipped
        >
          <v-timeline-item
            class="mb-4"
            color="grey"
            small
          >
            <v-row>
              <v-col cols="12">
                <span class="text-h4">2021 － 至今</span>
                <div class="content">
                  <p class="text-h6 mt-3">前端網頁開發技術/泰山職訓 <span class="text-subtitle-1 grey--text text--darken-2">泰山區</span></p>
                  <ul>
                    <li>學習前端各項技術如SASS、Bootstrap、Gsap、JavaScript、jQuery、Vue.js 等</li>
                    <li>前端簡易小遊戲、切版與作品集的製作</li>
                  </ul>
                </div>
              </v-col>
            </v-row>
          </v-timeline-item>
          <v-timeline-item
            class="mb-4 school"
            color="grey"
            small
          >
            <v-row>
              <v-col cols="12">
                <span class="text-h4">2015 － 2017</span>
                <div class="content">
                  <p class="text-h6 mt-3">臺北科技大學/材料所 <span class="text-subtitle-1 grey--text text--darken-2">台北市</span></p>
                  <ul>
                  <li>研究固態氧化物燃料電池摻雜不同元素的導電性</li>
                </ul>
                </div>
              </v-col>
            </v-row>
          </v-timeline-item>
          <v-timeline-item
            class="mb-4 school"
            color="grey"
            small
          >
            <v-row>
              <v-col cols="12">
                <span class="text-h4">2010 － 2015</span>
                <div class="content">
                  <p class="text-h6 mt-3">臺北科技大學/材料與資源工程學系<span class="text-subtitle-1 grey--text text--darken-2">台北市</span></p>
                  <ul>
                    <li>學習各種材料的特性與應用基礎理論</li>
                  </ul>
                </div>
              </v-col>
            </v-row>
          </v-timeline-item>
        </v-timeline>
      </v-col>
      <v-col cols="12" md="6">
        <p class="text-h4 my-10">經歷</p>
        <v-timeline
          dense
          clipped
        >
          <v-timeline-item
            class="mb-4"
            color="grey"
            small
          >
            <v-row>
              <v-col cols="12">
                <span class="text-h4">2018 － 2021</span>
                <div class="content">
                  <p class="text-h6 mt-3">製程工程師/勝麗國際公司 <span class="text-subtitle-1 grey--text text--darken-2">竹北市</span></p>
                  <ul class="grey--text text--darken-3">
                    <li>操作機台製作工程樣品、常與研發工程師(RD)與專案經理(PM)討論產品製作問題，並提出改善方案</li>
                    <li>與設備工程師(ME)一同解決線上機台生產異常排除與產線人員(OP)教育訓練</li>
                  </ul>
                </div>
              </v-col>
            </v-row>
          </v-timeline-item>
          <v-timeline-item
            class="mb-4"
            color="grey"
            small
          >
            <v-row>
              <v-col cols="12">
                <span class="text-h4">2017 － 2018</span>
                <div class="content">
                  <p class="text-h6 mt-3">技術服務/大鴻製釉有限公司 <span class="text-subtitle-1 grey--text text--darken-2">上海市</span></p>
                  <ul class="grey--text text--darken-3">
                    <li>提供顧客完善的技術服務，到紡織工廠內協助客戶使用墨水，並協助排除生產異常</li>
                    <li>測試研發工程師(RD)墨水配方上機後是否能生產流暢</li>
                  </ul>
                </div>
              </v-col>
            </v-row>
          </v-timeline-item>
        </v-timeline>
      </v-col>
    </v-row>
    <!-- 技能 -->
    <v-row id="skill">
      <v-col cols="12" class="mt-10">
        <p class="text-h4">技能</p>
      </v-col>
      <v-col cols="6" sm="4">
        <p class="text-h5">UI 框架</p>
        <v-divider></v-divider>
        <ul class="mt-4">
          <li>
            <v-icon left color="#8713F4">mdi-bootstrap</v-icon>
            Bootstrap
          </li>
          <li>
            <v-icon left color="#138FEA">mdi-vuetify</v-icon>
            Vuetify
          </li>
        </ul>
      </v-col>
      <v-col cols="6" sm="4" >
        <p class="text-h5">前端程式</p>
        <v-divider></v-divider>
        <ul class="mt-4">
          <li>
            <v-icon left color="#F1CB03">mdi-language-javascript</v-icon>
            JavaScript
          </li>
          <li>
            <v-icon left color="#0769AE">mdi-jquery</v-icon>
            jQuery
          </li>
          <li>
            <v-icon left color="#41B983">mdi-vuejs</v-icon>
            Vue.js
          </li>

        </ul>
      </v-col>
      <v-col cols="6" sm="4">
        <p class="text-h5">後端程式</p>
        <v-divider></v-divider>
        <ul class="mt-4">
          <li>
            <v-icon left color="#517429">mdi-nodejs</v-icon>
            Node.js
          </li>
          <li>
              <v-icon left color="#199F38">mdi-database</v-icon>
              MongoDB
          </li>
        </ul>
      </v-col>
      <v-col cols="6" sm="4">
        <p class="text-h5">工具</p>
        <v-divider></v-divider>
        <ul class="mt-4">
          <li>
            <v-icon left color="#F05033">mdi-git</v-icon>
            git
          </li>
        </ul>
      </v-col>
    </v-row>
    <v-row id="portfolio">
      <v-col cols="12" class="mt-10">
        <p class="text-h4">作品集</p>
      </v-col>
      <v-col cols="12" sm="6" md="4">
        <v-card :ripple="false" href="https://raquelyang.github.io/purecrop/#/">
          <v-img
            src="../assets/images/purecrop.jpg"
            class="white--text align-end"
            height="200px"
          >
          </v-img>
          <v-card-text class="text--primary py-0">
            <v-card-title class="px-0 pb-5">
              無疑農
              <v-spacer></v-spacer>
              <v-btn icon href="https://github.com/RaquelYang/purecrop">
                <v-icon>mdi-github</v-icon>
              </v-btn>
            </v-card-title>
            <v-card-subtitle class="px-0">簡易小農購物網站，包括登入、註冊、新增商品等連接後端資料庫，並嵌入 Google Analytics </v-card-subtitle>
            <v-chip class="mb-3 mr-2">Vue</v-chip>
            <v-chip class="mb-3 mr-2">Vuetify</v-chip>
            <v-chip class="mb-3 mr-2">mongoDB</v-chip>
          </v-card-text>
        </v-card>
      </v-col>
      <v-col cols="12" sm="6" md="4">
        <v-card :ripple="false">
          <v-img
            src="../assets/images/michelin.jpeg"
            class="white--text align-end"
            gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.2)"
            height="200px"
          >
          </v-img>
          <v-card-text class="text--primary py-0">
            <v-card-title class="px-0 pb-5">
              米其林餐廳 Linebot
              <v-spacer></v-spacer>
              <v-btn icon href="https://github.com/RaquelYang/linebot_homework-D">
                <v-icon>mdi-github</v-icon>
              </v-btn>
            </v-card-title>
            <v-card-subtitle class="px-0">使用 RESTful API 串接米其林餐廳官網外部資料，並整合 Line 機器人查找餐廳 ID:@488pghgt</v-card-subtitle>
            <v-chip class="mb-3 mr-2">Node.js</v-chip>
            <v-chip class="mb-3 mr-2">linebot</v-chip>
          </v-card-text>
        </v-card>
      </v-col>
      <v-col cols="12" sm="6" md="4">
        <v-card :ripple="false"  href="">
          <v-img
            @click="gotogitpage('https://raquelyang.github.io/pomodoro1/#/')"
            src="../assets/images/tomato.svg"
            class="white--text align-end cursor"
            gradient="to bottom, rgba(0,0,0,.05), rgba(0,0,0,.15)"
            height="200px"
          >
          </v-img>
          <v-card-text class="text--primary py-0">
            <v-card-title class="px-0 pb-5">
              番茄鐘
              <v-spacer></v-spacer>
              <v-btn icon href="https://github.com/RaquelYang/pomodoro1">
                <v-icon>mdi-github</v-icon>
              </v-btn>
            </v-card-title>
            <v-card-subtitle class="px-0">使用 F2E 設計稿切版、設計番茄鐘功能，並部署 PWA 製成簡易網路應用程式</v-card-subtitle>
            <v-chip class="mb-3 mr-2">Vue</v-chip>
            <v-chip class="mb-3 mr-2">SCSS</v-chip>
          </v-card-text>
        </v-card>
      </v-col>
    </v-row>
    </v-container>

  </div>
</template>
<style lang="scss">
#home{
  margin-bottom: 5rem;
  .theme--light.v-list-item--disabled{
    color:#333
  }
  .nav{
    backdrop-filter: blur(10px);
    background-color: transparent;
    justify-content: center;
    align-items: center;
    a{
      margin: 0 1rem;
      opacity: .8;
      &:hover{
        opacity: 1;
      }
    }
  }
  .name a{
    color:#333
  }
  .maincontent{
    // margin: 3rem 0;
    margin-top: 3rem;
    background-color: white;
    box-shadow: 0px 5px 20px rgba(0,0,0,.1);
  }
  .v-divider {
    border-width: medium 0 0 0;
  }
  a{
    text-decoration: none;
  }
  .v-timeline-item{
    padding-bottom:15rem;
    position: relative;
  }
  .v-timeline-item.school{
    padding-bottom:10rem;
  }
  .content{
    position: absolute;
  }
  li{
    font-size: 1.2rem;
    padding: 0.5rem 0;
    list-style: none;
    vertical-align: middle;
    position: relative;
  }
  #educationandexperience{
    li{
      &::before{
      content:'➤';
      position: absolute;
      display:block;
      color: #666;
      top:8px;
      left: -22px;
    }
    }
  }
  .portfolio p{
    line-height: 1.4rem;
    letter-spacing: 1px;
  }
  .cursor{
    cursor: pointer;
  }
}
</style>
<script>
export default {
  data () {
    return {
      drawer: false
    }
  },
  methods: {
    gotogitpage (url) {
      window.location.href = url
    }
  }
}
</script>
