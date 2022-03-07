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
    class="navbar"
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
              <v-img src="../assets/images/self2.jpg" class="rounded px-16 py-16 img"></v-img>
            </v-col>
            <v-col cols="12">
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
      <v-col cols="12" sm="12" md="12">
          <v-card class="purecrop">
            <v-row class="py-5 px-5">
              <v-col cols="12" sm="6">
                <v-img class="cursor" src="../assets/images/purecrop.jpg" @click="gotogitpage('https://raquelyang.github.io/Purecrop/#/')"></v-img>
              </v-col>
              <v-col cols="12" sm="6" class="d-flex flex-column justify-space-between">
                <div>
                  <h3 class="text-h4">無疑農 Purecrop</h3>
                  <p class="pt-5">小農購物網站，包括會員(管理員)登入、註冊、管理員商品與輪播圖的增改刪查、訂單狀態變更等功能。資料庫使用 mongoDB ，並嵌入 Google Analytics 可分析使用者點擊狀態。</p>
                </div>
                <div>
                  <v-chip class="mb-3 mr-2">Vue</v-chip>
                  <v-chip class="mb-3 mr-2">Vuetify</v-chip>
                  <v-chip class="mb-3 mr-2">SCSS</v-chip>
                  <v-chip class="mb-3 mr-2">Node.js</v-chip>
                  <v-chip class="mb-3 mr-2">mongoDB</v-chip>
                </div>
              </v-col>
              <v-col cols="12" sm="6">
                <p class="text-h5">前端</p>
                <ul class="text-subtitle-1">
                  <li>Vue 前端框架搭配 Vuetify </li>
                  <li>Vuex 管理前端狀態</li>
                  <li>Axios 向後端伺服器請求資料</li>
                  <li>註冊與登入功能</li>
                  <li>管理員資料修改</li>
                </ul>
              </v-col>
              <v-col cols="12" sm="6">
                <p class="text-h5">後端</p>
                <ul class="text-subtitle-1">
                  <li>Node.js 搭配 Express.js 建立伺服器</li>
                  <li>MongoDB 作為後端資料庫，管理產品、輪播圖增改刪查刪查</li>
                </ul>
              </v-col>
            </v-row>
          </v-card>
      </v-col>
      <v-col cols="12" sm="6" md="4">
        <v-card :ripple="false" height="400px">
          <v-img
            src="../assets/images/michelin.jpeg"
            class="white--text align-end"
            gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.2)"
            height="200px"
          >
          </v-img>
          <v-card-text class="card text--primary py-0 d-flex flex-column justify-space-between">
            <div>
              <v-card-title class="px-0 pb-5">
              米其林餐廳 Linebot
              <v-spacer></v-spacer>
              <v-btn icon href="https://github.com/RaquelYang/linebot_homework-D">
                <v-icon>mdi-github</v-icon>
              </v-btn>
            </v-card-title>
            <v-card-subtitle class="px-0">使用 RESTful API 串接米其林餐廳官網外部資料，並整合 Line 機器人查找餐廳 ID:@488pghgt</v-card-subtitle>
            </div>
            <div>
              <v-chip class="mb-3 mr-2">Node.js</v-chip>
              <v-chip class="mb-3 mr-2">linebot</v-chip>
            </div>
          </v-card-text>
        </v-card>
      </v-col>
      <v-col cols="12" sm="6" md="4">
        <v-card :ripple="false" height="400px">
          <v-img
            @click="gotogitpage('https://raquelyang.github.io/pomodoro1/#/')"
            src="../assets/images/tomato.svg"
            class="white--text align-end cursor"
            gradient="to bottom, rgba(0,0,0,.05), rgba(0,0,0,.15)"
            height="200px"
          >
          </v-img>

          <v-card-text class="text--primary py-0 card d-flex flex-column justify-space-between">
            <div>
              <v-card-title class="px-0 pb-5">
              番茄鐘
              <v-spacer></v-spacer>
              <v-btn icon href="https://github.com/RaquelYang/pomodoro1">
                <v-icon>mdi-github</v-icon>
              </v-btn>
            </v-card-title>
            <v-card-subtitle class="px-0">使用 F2E 設計稿切版、設計番茄鐘功能，其使用 Vue 組件間通信並部署 PWA 製成簡易網路應用程式</v-card-subtitle>
            </div>
            <div>
              <v-chip class="mb-3 mr-2">HTML</v-chip>
              <v-chip class="mb-3 mr-2">SCSS</v-chip>
              <v-chip class="mb-3 mr-2">Vue</v-chip>
            </div>
          </v-card-text>
        </v-card>
      </v-col>
      <v-col cols="12" sm="6" md="4">
        <v-card :ripple="false" height="400px">
          <v-img
            @click="gotogitpage('https://raquelyang.github.io/Typinggame/')"
            src="../assets/images/typinggame.jpg"
            class="white--text align-end cursor"
            gradient="to bottom, rgba(0,0,0,.05), rgba(0,0,0,.15)"
            height="200px"
          >
          </v-img>
          <v-card-text class="text--primary py-0 card d-flex flex-column justify-space-between">
            <div>
              <v-card-title class="px-0 pb-5">
              打字小遊戲
              <v-spacer></v-spacer>
              <v-btn icon href="https://github.com/RaquelYang/Typinggame">
                <v-icon>mdi-github</v-icon>
              </v-btn>
              </v-card-title>
            <v-card-subtitle class="px-0">使用 jQuery 製作練習打英文字母的小遊戲，成功打完一個字就加一分，會顯示排行前五名的選手名稱。</v-card-subtitle>
            </div>
            <div>
              <v-chip class="mb-3 mr-2">HTML</v-chip>
              <v-chip class="mb-3 mr-2">CSS</v-chip>
              <v-chip class="mb-3 mr-2">jQuery</v-chip>
            </div>
          </v-card-text>
        </v-card>
      </v-col>
      <v-col cols="12" sm="6" md="4">
        <v-card :ripple="false" height="400px">
          <v-img
            @click="gotogitpage('https://raquelyang.github.io/card-game/')"
            src="../assets/images/popcorn.png"
            class="white--text align-end cursor"
            gradient="to bottom, rgba(0,0,0,.05), rgba(0,0,0,.15)"
            height="200px"
          >
          </v-img>
          <v-card-text class="text--primary py-0 card d-flex flex-column justify-space-between">
            <div>
              <v-card-title class="px-0 pb-5">
              爆米花點擊遊戲
              <v-spacer></v-spacer>
              <v-btn icon href="https://github.com/RaquelYang/popcorn">
                <v-icon>mdi-github</v-icon>
              </v-btn>
              </v-card-title>
            <v-card-subtitle class="px-0">使用 jQuery 製作爆米花點擊小遊戲，成功點擊爆米花加一分，點擊玉米粒則扣一分，時間結束後會顯示分數。</v-card-subtitle>
            </div>
            <div>
              <v-chip class="mb-3 mr-2">HTML</v-chip>
              <v-chip class="mb-3 mr-2">CSS</v-chip>
              <v-chip class="mb-3 mr-2">jQuery</v-chip>
            </div>
          </v-card-text>
        </v-card>
      </v-col>
      <v-col cols="12" sm="6" md="4">
        <v-card :ripple="false" height="400px">
          <v-img
            @click="gotogitpage('https://raquelyang.github.io/bootstrap-layout/')"
            src="../assets/images/bootstrap.png"
            class="white--text align-end cursor"
            gradient="to bottom, rgba(0,0,0,.05), rgba(0,0,0,.15)"
            height="200px"
          >
          </v-img>
          <v-card-text class="text--primary py-0 card d-flex flex-column justify-space-between">
            <div>
              <v-card-title class="px-0 pb-5">
              Bootstrap 切版
              <v-spacer></v-spacer>
              <v-btn icon href="https://github.com/RaquelYang/bootstrap-layout">
                <v-icon>mdi-github</v-icon>
              </v-btn>
              </v-card-title>
            <v-card-subtitle class="px-0">使用 bootstrap 切兩欄、三欄、滿版與輪播圖，並有RWD 功能</v-card-subtitle>
            </div>
            <div>
              <v-chip class="mb-3 mr-2">HTML</v-chip>
              <v-chip class="mb-3 mr-2">Bootstrap</v-chip>
            </div>
          </v-card-text>
        </v-card>
      </v-col>
      <v-col cols="12" sm="6" md="4">
        <v-card :ripple="false" height="400px">
          <v-img
            @click="gotogitpage('https://raquelyang.github.io/templateMonster/')"
            src="../assets/images/templateMonster.png"
            class="white--text align-end cursor"
            gradient="to bottom, rgba(0,0,0,.05), rgba(0,0,0,.15)"
            height="200px"
          >
          </v-img>
          <v-card-text class="text--primary py-0 card d-flex flex-column justify-space-between">
            <div>
              <v-card-title class="px-0 pb-5">
              Construction 切版(純 CSS )
              <v-spacer></v-spacer>
              <v-btn icon href="https://github.com/RaquelYang/templateMonster">
                <v-icon>mdi-github</v-icon>
              </v-btn>
              </v-card-title>
            <v-card-subtitle class="px-0">參考 bootstrap 格線系統切，從 TemplateMonster 網站中挑選樣板，並做出 RWD 功能</v-card-subtitle>
            </div>
            <div>
              <v-chip class="mb-3 mr-2">HTML</v-chip>
              <v-chip class="mb-3 mr-2">CSS</v-chip>
              <v-chip class="mb-3 mr-2">JavaScript</v-chip>
            </div>
          </v-card-text>
        </v-card>
      </v-col>
    </v-row>
    </v-container>

  </div>
</template>
<style lang="scss">
#home{
  background-color: #eee;
  padding: 6rem 0;
  .purecrop {
    p{
    letter-spacing: .1rem;
    line-height: 1.8;
    }
    li{
      font-size: 1.1rem;
      &::before{
      content:'➤';
      position: absolute;
      display:block;
      color: #666;
      top:8px;
      left: -25px;
      }
    }
  }
  .card{
    height: 50%;
  }
  .theme--light.v-list-item--disabled{
    color:#333
  }
  .navbar{
    backdrop-filter: blur(10px);
    background-color: rgba(255, 255, 255, 0.3);
    .nav{
      justify-content: center;
      align-items: center;
    }
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
    border-radius: .2rem;
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
    line-height: 1.8;
    letter-spacing: 2px;
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
