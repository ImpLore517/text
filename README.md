<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta name="title" content="達康.come">
    <meta name="description" content="【達康.come】成立於2013年初，阿達、康康兩人從事專職搞笑、漫才表演歷時10年多。">
    <meta name="keywords" content="達康.come, 達康, 阿達, 康康">
    <title>達康.come</title>
    <link rel="stylesheet" href="style.css" />
    <link rel="icon" href="./logo.jpg">
    <link
      rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css"
    />
    <!-- <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/css/bootstrap.min.css" -->
    <!-- integrity="sha384-rbsA2VBKQhggwzxH7pPCaAqO46MgnOM80zW1RWuH61DGLwZJEdK2Kadq2F9CUG65" crossorigin="anonymous"> -->
  </head>

  <body>
    <div id="app">
      <!-- nav -->
      <nav>
        <div class="nav-content">
          <a href="#home" @click.prevent="toTitle">
            <img src="./logo.jpg" class="logo" />
          </a>
          <a href="#about-dacon" @click.prevent="toTitle" class="nav-text">
            <i class="fa-solid fa-user"></i>
            關於達康
          </a>
          <a href="#manzai" @click.prevent="toTitle" class="nav-text">
            <i class="fa-solid fa-comment"></i>
            漫才介紹
          </a>
          <a href="#perform" @click.prevent="toTitle" class="nav-text">
            <i class="fa-solid fa-video"></i>
            相關作品
          </a>
          <a href="#sell" @click.prevent="toTitle" class="nav-text">
            <i class="fa-solid fa-ticket"></i>
            售票資訊
          </a>
          <div class="links">
            <a href="https://www.facebook.com/dacon.come">
              <i class="fa-brands fa-facebook"></i>
            </a>
            <a href="https://www.instagram.com/dacon.come/">
              <i class="fa-brands fa-instagram ml-1"></i>
            </a>
            <a href="https://www.youtube.com/@dacondacome">
              <i class="fa-brands fa-youtube ml-1"></i>
            </a>
          </div>
        </div>
      </nav>
      <div class="cover"></div>
      <!-- picture -->
      <div class="picture" id="home">
        <div class="slide" v-for="(item,key) in pictures" :key="key">
          <img :src="item.img" />
        </div>
      </div>
      <!-- section1 -->
      <section class="container" id="about-dacon">
        <div class="title">
          <h1 class="mb-1">關於達康</h1>
          <p>
            達康.come是由陳彥達（阿達）和何瑞康（康康）組成的台灣漫才搭檔組合，於2013年創立笑太夫漫才集團，由阿達（陳彥達）擔任團長，康康（何瑞康）擔任劇團總監，以推廣漫才創作、演出作為劇團的重點核心，並嘗試運用各種戲劇特性，結合漫才精神，發展各類型喜劇表現樣貌，未來更朝漫才發展之情境喜劇結合各種媒體運用為目標，期待讓表演更豐富，為觀眾帶來更多歡笑。
          </p>
          <br />
          <p>
            陳彥達自2007年起從事搞笑相關創作及演出，曾任魚蹦興業副團長。何瑞康自2008年起從事搞笑相關創作及演出，曾是魚蹦興業團員，也是位踢踏舞者、吉他手、歌手、詞曲創作者。兩人皆為國立臺北藝術大學戲劇系畢業，是學長和學弟的關係。2013年初兩人結成搭檔，初期團名為「黃金比例」，陳彥達擔任團長，何瑞康擔任劇團總監，寫段子、排練到演出都是兩人包辦。
          </p>
        </div>
        <div class="content">
          <img src="./ada.jpg" class="people" />
          <div class="content-text">
            <h2 class="mb-1">陳彥達（阿達）</h2>
            <p>
              自2008年起從事日式漫才、搞笑創作及演出至今，2013年與何瑞康共同組成漫才搞笑組合「達康.come」，除每年自製2至4檔創作演出，也受邀至各藝術節製作演出節目，如臺北藝術節《達康宅配便》、TIFA台灣國際藝術節《活屍末日劇院求生指南》、果陀爆米花劇場2.0《塾話說得好》、3.0《我是笑星》、4.0《走味關係》，亦曾參與電視情境喜劇《原來一家人》編劇工作。
            </p>
            <br />
            <p>
              於2015為尋求更多有志於漫才表演的夥伴，開設「達康.come漫才塾」進行為期半年的漫才、日式搞笑課程，學員結業後組成「漫！！男塾」活動至今。
            </p>
            <br />
            <p>
              達康.come自製結合網路播送的現場搞笑節目《好了啦！達康》，目前進行至第七季。也曾於阮劇團《熱天酣眠》、《嫁妝一牛車》、日本吉本興業短篇電影《選ばれた男》擔任演員，夾腳拖劇團《阿嬤的雜細車》擔任導演。
            </p>
          </div>
        </div>
        <div class="content">
          <img src="./kangkang.jpg" class="people" />
          <div class="content-text">
            <h2 class="mb-1">何瑞康（康康）</h2>
            <p>
              從事劇場表演與創作。於喜劇領域耕耘13年，創作平台從劇場到影視媒介，以編劇以及表演擅長。受邀至國家戲劇院、臺北藝術節、果陀劇場、各地方劇院等單位公演，並為台灣當地電視節目製作公司編寫長篇情境喜劇。2018開始實驗於網路直播媒介發表LIVE喜劇節目《好了啦！達康》。
            </p>
            <br />
            <p>
              從事節奏踢踏舞表演，多次前往日本及美國進修，曾受邀至日本東京踢踏節、臺北踢踏節、臺北白晝之夜等活動中演出，並與本地爵士樂團合作舉辦音樂表演。亦將踢踏舞的節奏即興與身體表達等思考為主軸，與其他劇場導演合作並演出。
            </p>
            <br />
            <p>
              2014開始投入個人音樂作品創作及演唱，於2016錄製發行首張EP《給我說個故事吧》，於2019年底發行個人首張創作專輯《山那》。
            </p>
          </div>
        </div>
      </section>
      <!-- section2 -->
      <section class="container" id="manzai">
        <h1 class="border-blue">漫才介紹</h1>
        <div class="content align-center">
          <div class="content-text">
            <ul>
              <li>
                <h2 class="mb-1">漫才</h2>
                <p>
                  漫才（日語：漫才／まんざいManzai）是日本的一種喜劇表演形式，前身是日本古代傳統藝能的萬歲。受到愛知縣尾張萬歲與三河萬歲的影響，在日本關西地區漸漸發展出這種表演形式。在1933年，吉本興業將這種表演方式改稱為漫才，並推廣到全日本。
                </p>
                <br />
                <p>
                  漫才在近代經常被認為與大阪地區有所關連，而漫才表演者（漫才師）也通常以關西口音演出。漫才大多由兩人組合演出，一人擔任較滑稽的角色負責裝傻（ボケ），另一人擔任較嚴肅的角色負責吐槽（ツッコミ），兩人藉由彼此的互動去講述笑話。大部分的笑點圍繞在兩人之間的誤會、雙關語和諧音字詞。演出方式與中國的對口相聲、西方的雙人搭檔相似。
                </p>
                <br />
                <p>
                  漫才的題材往往與日常生活有關。有時喜劇演員會向觀眾提問，有時漫才師會根據觀眾的反應添加幾行對話。因此，漫才的特點是表演者不僅做自己想做的事情，而且觀眾的反應也是表演的一部分。
                </p>
              </li>
              <li>
                <br />
                <br />
                <h2 class="mb-1">歷史</h2>
                <p>
                  一般認為漫才是來自「萬歲」，後逐漸用「萬」的同音字「漫」（日文都讀作「まん」，即「man」）和「歲」在日語中的俗體字「才」代替，才慢慢形成「漫才」的寫法。萬歲是從平安時代開始的藝能表演，是指在新年表示祝福話語的歌舞。以兩人為一組造訪各家戶，在說出新年的祝福話語後，其中一人開始打鼓，另一人則開始跳舞。在江戶時代，依據各地方的風格不同，出現了加上地名各種萬歲表演形態，例如尾張萬歲、三河萬歲等。之後流行的大和萬歲，是在歌舞和祝福話語之外加上猜謎、問答等趣味性的滑稽談話，漸漸發展成主流的形式。1933年，大阪發跡的娛樂表演集團吉本興業首次提出漫才的定義，並將這一種新類型的喜劇帶往東京，但是第二次世界大戰後這項表演漸漸衰退。直到1970年代的漫才熱潮才開始漸漸流行起來。2001年起至今（中間停辦5年）每年一度、由吉本興業主辦的M-1大賽，以競爭一千萬日元賞金的比賽形式，將漫才這種表演形式提高到新的高度。
                </p>
              </li>
            </ul>
          </div>
          <img src="./manzai.jpg" alt="maizai" />
        </div>
        <div class="content-text">
          <h2 class="mb-1">漫才、相聲的不同之處</h2>
          <div class="dif-video">
            <iframe
              width="560"
              height="315"
              src="https://www.youtube.com/embed/wwqxR3Zi1xo"
              title="YouTube video player"
              frameborder="0"
              allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
              allowfullscreen
            ></iframe>
            <iframe
              width="560"
              height="315"
              src="https://www.youtube.com/embed/gdkLmkNkY8E"
              title="YouTube video player"
              frameborder="0"
              allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
              allowfullscreen
            ></iframe>
          </div>
        </div>
      </section>
      <!-- section3 -->
      <section class="container" id="perform">
        <h1 class="mb-1">相關作品</h1>
        <!-- 好了啦！達康 -->
        <h2 class="mb-1">好了啦！達康</h2>
        <p>
          精心編排笑料不間斷的「漫才」
          由你來出題考驗反應力的「即興節目」歌詞永遠沒道理但旋律總是那麼好聽的「晚安曲」
          《好了啦》一次都給你！
        </p>
        <div class="video mb-2 mt-1">
          <button
            type="submit"
            class="side-arrow"
            @click="moveLeft('.itsOkVideo','.itsOkPage')"
          >
            <i class="fa-solid fa-chevron-left"></i>
          </button>
          <div class="content-video">
            <div class="itsOkVideo" v-for="(item,key) in itsOk" :key="key">
              <iframe
                width="560"
                height="315"
                :src="item.video"
                title="YouTube video player"
                frameborder="0"
                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                allowfullscreen
              ></iframe>
            </div>
          </div>
          <button
            type="submit"
            class="side-arrow"
            @click="moveRight('.itsOkVideo','.itsOkPage')"
          >
            <i class="fa-solid fa-chevron-right"></i>
          </button>
          <div class="selector itsOkPage" @click="choose"></div>
        </div>
        <!-- 還在講 -->
        <h2 class="mb-1">達康還在講</h2>
        <p>
          達康.come加上好朋友哈利的Podcast節目，每週選聊話題，陪伴你度過不無聊的上班、通勤、開車，你的耳裡隨時有阿達康康與哈利魔性的笑聲。
        </p>
        <div class="video mb-2 mt-1">
          <button
            type="submit"
            class="side-arrow"
            @click="moveLeft('.stillTalkVideo','.stillTalkPage')"
          >
            <i class="fa-solid fa-chevron-left"></i>
          </button>
          <div class="content-video">
            <div
              class="stillTalkVideo"
              v-for="(item,key) in stillTalk"
              :key="key"
            >
              <iframe
                width="560"
                height="315"
                :src="item.video"
                title="YouTube video player"
                frameborder="0"
                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                allowfullscreen
              ></iframe>
            </div>
          </div>
          <button
            type="submit"
            class="side-arrow"
            @click="moveRight('.stillTalkVideo','.stillTalkPage')"
          >
            <i class="fa-solid fa-chevron-right"></i>
          </button>
          <div class="selector stillTalkPage" @click="choose"></div>
        </div>
        <!-- 集合囉！Play Boy Station！ -->
        <h2 class="mb-1">集合囉！Play Boy Station！</h2>
        <p><span class="xbox">△</span> 達康.come ＆ 漫才少爺（まんざいぼんぼん）</p>

        <p><span class="xbox">▢</span> 台日漫才師聯手出擊</p>

        <p><span class="xbox">◯</span> 全新遊戲企劃型節目</p>

        <p><span class="xbox">⨯</span> 每個月給你全新笑料</p>

        <div class="video mb-2 mt-1">
          <button
            type="submit"
            class="side-arrow"
            @click="moveLeft('.PBSVideo','.PBSPage')"
          >
            <i class="fa-solid fa-chevron-left"></i>
          </button>
          <div class="content-video">
            <div class="PBSVideo" v-for="(item,key) in PBS" :key="key">
              <iframe
                width="560"
                height="315"
                :src="item.video"
                title="YouTube video player"
                frameborder="0"
                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share "
                allowfullscreen
              ></iframe>
            </div>
          </div>
          <button
            type="submit"
            class="side-arrow"
            @click="moveRight('.PBSVideo','.PBSPage')"
          >
            <i class="fa-solid fa-chevron-right"></i>
          </button>
          <div class="selector PBSPage" @click="choose"></div>
        </div>
      </section>
      <!-- section4 -->
      <section class="container" id="sell">
        <h1 class="border-blue">售票資訊</h1>
        <div class="content ml-2">
          <img src="s7e2.png" class="ticket-img" />
          <div class="content-text">
            <h2 class="mb-1 circle-font">《好了啦！達康！》第七季第二集</h2>
            <h2 class="mb-1 circle-font">D.C. Night Live</h2>
            <p>類別：戲劇</p>
            <p>分級：建議年齡 12歲以上</p>
            <p>時間：2023/3/31 (五) - 2023/4/22 (六)</p>
            <p>主辦：笑太夫漫才集團 02-28212426</p>
            <p>地點：臺北 → 中影八德大樓演講廳</p>
            <p class="text-indent-5">高雄 → 高雄市文化中心至善廳</p>
            <p class="text-indent-5">臺中 → 國立臺中教育大學寶成演藝廳</p>
            <p>
              購票網址：<a href="https://reurl.cc/AdA3jp" target="_blank"
                >https://reurl.cc/AdA3jp</a
              >
            </p>
          </div>
        </div>
        <div class="content ml-2">
          <img src="Yuntech.jpeg" class="ticket-img" />
          <div class="content-text">
            <h2 class="mb-1 circle-font">達康.COME笑現場IN雲泰表演廳</h2>
            <h2 class="mb-1 circle-font">
              Dacon.come laughing live show in Yuntay Performance Hall
            </h2>
            <p>類別：戲劇</p>
            <p>分級：建議年齡 7歲以上</p>
            <p>時間：2023/4/27 (四) 19:30</p>
            <p>主辦：國立雲林科技大學 05-5342601分機2458</p>
            <p>地點：國立雲林科技大學-雲泰表演廳</p>
            <p>
              購票網址：<a href="https://reurl.cc/o07YEj" target="_blank"
                >https://reurl.cc/o07YEj</a
              >
            </p>
          </div>
        </div>
        <div class="content ml-2">
          <img src="guest.png" class="ticket-img" />
          <div class="content-text">
            <h2 class="mb-1 circle-font">傻孩子宅急便《這個殺手不太妙plus》</h2>
            <h2 class="mb-1 circle-font">
              Ahogakitakkyubin" Dumb Dumb Hit Man plus "
            </h2>
            <p>類別：戲劇</p>
            <p>分級：保護級</p>
            <p>時間：2023/5/6 (六) - 2023/5/14 (日)</p>
            <p>主辦：你好漫才工作室 0971-071-952</p>
            <p>地點：PLAYground 南村劇場．青鳥．有.設計</p>
            <p>備註：達康.come為2023/5/6(六)兩場的<span class="important">特邀嘉賓</span></p>
            <p>
              購票網址：<a href="https://reurl.cc/klX80d" target="_blank"
                >https://reurl.cc/klX80d</a
              >
            </p>
          </div>
        </div>
      </section>
      <!-- footer -->
      <footer>
        <p>僅個人學習使用，無任何商業用途</p>
      </footer>
      <!-- back to top -->
      <a href="#home" @click.prevent="toTitle" class="top-arr">
        <i class="fas fa-arrow-up"></i>
      </a>
    </div>

    <script src="https://unpkg.com/vue@3/dist/vue.global.js"></script>
    <script type="module">
      import {
        createApp,
        ref,
        computed,
        onMounted,
      } from 'https://cdnjs.cloudflare.com/ajax/libs/vue/3.2.45/vue.esm-browser.min.js';
      const app = createApp({
        setup() {
          // 大圖
          const pictures = ref([
            {
              img: './action1.jpeg',
            },
            {
              img: './action2.jpg',
            },
            {
              img: './action3.jpg',
            },
            {
              img: './action4.jpeg',
            },
            {
              img: './action5.jpeg',
            },
          ]);
          // 大圖移動
          onMounted(() => {
            const slides = document.querySelectorAll('.slide');
            slides.forEach(function (slide, index) {
              slide.style.left = `${index * 100}%`;
            });
            let counter = 0;
            function transform() {
              counter++;
              const slides = document.querySelectorAll('.slide');
              slides.forEach(function (slide) {
                slide.style.transform = `translateX(-${counter * 100}%)`;
              });
              if (counter > pictures.value.length - 2) {
                counter = 0;
              }
            }
            setInterval(transform, 6000);
          });
          // scrollTo
          function toTitle(e) {
            const id = e.currentTarget.getAttribute('href').slice(1);
            const element = document.getElementById(id).offsetTop;
            const position = element - 80;

            window.scrollTo({
              top: position,
              left: 0,
            });
          }
          // 好了啦！達康
          const itsOk = ref([
            {
              video: 'https://www.youtube.com/embed/yI0h4FiOeGk',
            },
            {
              video: 'https://www.youtube.com/embed/KhI5-k7un4s',
            },
            {
              video: 'https://www.youtube.com/embed/GeSXs7jnLXY',
            },
            {
              video: 'https://www.youtube.com/embed/YAYHco_JfEQ',
            },
            {
              video: 'https://www.youtube.com/embed/n-U-Oln3bfE',
            },
          ]);
          // 達康還在講
          const stillTalk = ref([
            {
              video: 'https://www.youtube.com/embed/ZWl5Hedwq1A',
            },
            {
              video: 'https://www.youtube.com/embed/2oGO1Ui-IWs',
            },
            {
              video: 'https://www.youtube.com/embed/LBb-foPGyqU',
            },
            {
              video: 'https://www.youtube.com/embed/V410xZFJb5A',
            },
            {
              video: 'https://www.youtube.com/embed/pOallxogDZc',
            },
            {
              video: 'https://www.youtube.com/embed/PiDviAgFtJQ',
            },
          ]);
          // PBS
          const PBS = ref([
            {
              video: 'https://www.youtube.com/embed/WHeDUoAtu40',
            },
            {
              video: 'https://www.youtube.com/embed/utFMNT3TLjM',
            },
            {
              video: 'https://www.youtube.com/embed/y3cv19hZDwA',
            },
            {
              video: 'https://www.youtube.com/embed/HAIrQFmGjjc',
            },
            {
              video: 'https://www.youtube.com/embed/agRqpQmNLHE',
            },
          ]);
          // 影片左右移、影片頁面選擇點
          onMounted(() => {
            const itsOkVideos = document.querySelectorAll('.itsOkVideo');
            const itsOkPage = document.querySelector('.itsOkPage');
            const stillTalkVideos =
              document.querySelectorAll('.stillTalkVideo');
            const stillTalkPage = document.querySelector('.stillTalkPage');
            const PBSVideos = document.querySelectorAll('.PBSVideo');
            const PBSPage = document.querySelector('.PBSPage');
            function setVideo(video, page) {
              video.forEach(function (e, index) {
                e.style.left = `${index * 50}%`;
              });

              // 影片下方頁面選擇點
              const length = Math.ceil(video.length / 2);
              const arr = new Array(length).fill('');
              const arr1 = arr
                .map(function (text, index) {
                  return `<button type="button" class="circle-btn" data-id="${index}">${text}</button>`;
                })
                .join('');
              page.innerHTML = arr1;

              const circle = page.childNodes;
              circle[0].classList.add('bg-black');
            }

            setVideo(itsOkVideos, itsOkPage);
            setVideo(stillTalkVideos, stillTalkPage);
            setVideo(PBSVideos, PBSPage);
          });
          let counter = 0;
          function moveRight(video, page) {
            const element = document.querySelectorAll(video);
            const x =
              element[2].getBoundingClientRect().x -
              element[0].getBoundingClientRect().x;
            if (counter < Math.floor((element.length - 1) / 2)) {
              counter++;
            }
            element.forEach((video, index) => {
              video.style.transform = `translateX(-${counter * x}px)`;
            });

            const circle = document.querySelector(page).childNodes;
            circle.forEach(function (circle) {
              circle.classList.remove('bg-black');
            });

            circle[counter].classList.add('bg-black');
          }
          function moveLeft(video, page) {
            const element = document.querySelectorAll(video);
            const x =
              element[2].getBoundingClientRect().x -
              element[0].getBoundingClientRect().x;
            if (counter > 0) {
              counter--;
            } else {
              counter = 0;
            }
            element.forEach((video, index) => {
              video.style.transform = `translateX(-${counter * x}px)`;
            });

            const circle = document.querySelector(page).childNodes;
            circle.forEach(function (circle) {
              circle.classList.remove('bg-black');
            });

            circle[counter].classList.add('bg-black');
          }
          // 選擇點換頁
          function choose(e) {
            const data = e.path[0].dataset.id;
            const videos = [...e.path[2].childNodes[1].childNodes].slice(1, -1);
            videos.forEach((video) => {
              video.style.transform = `translateX(-${data * 1567}px)`;
            });
            const circles = e.path[1].childNodes;
            circles.forEach((circle) => {
              circle.classList.remove('bg-black');
            });
            circles[data].classList.add('bg-black');
            counter = data;
          }
          // back-to-top-arr
          window.addEventListener('scroll', function () {
            const height = window.pageYOffset;
            if (height > 500) {
              document.querySelector('.top-arr').classList.add('show-arr');
            } else {
              document.querySelector('.top-arr').classList.remove('show-arr');
            }
          });

          return {
            pictures,
            itsOk,
            stillTalk,
            PBS,
            counter,
            toTitle,
            moveLeft,
            moveRight,
            choose,
          };
        },
      });
      app.mount('#app');
    </script>
  </body>
</html>
