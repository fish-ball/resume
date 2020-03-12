<template>
  <div class="container">
    <div class="sidebar">
      <div class="block-title">
        <div class="avatar">
          <img class="avatar" src="@/assets/images/avatar.png" />
        </div>
        <h1 class="name">
          <span class="primary">{{r.name.primary}}</span> /
          <span class="secondary">{{r.name.secondary}}</span>
        </h1>
        <div class="origin">{{r.origin.year}}年 {{r.origin.location}}</div>
        <div class="position">{{r.position}}</div>
      </div>
      <div class="block-introduction">
        <section class="section section-introduction">
          <h2 class="section-title">个人介绍</h2>
          <div class="section-body">
            <ul class="item-list disc">
              <li>经验丰富：编程经验15年，从事软件行业10年以上，其中金融业5年，自主创业6年。</li>
              <li>基础扎实：数学与编程算法基础扎实，学习期间多次获得重要奖项。</li>
              <li>技能全面：创业期间已经熟练掌握各类前后端主流开发技能。</li>
              <li>团队管理：创业期间带领过10人的团队，熟悉软件开发项目的分工与管理。</li>
              <li>熟悉运营：熟悉软件项目的技术运营，掌握各种主流的部署架构以及容器化部署与运营。</li>
              <li>追求卓越：能够把握工作重点，目的性强，习惯于找到最合理的方式解决问题。</li>
            </ul>
          </div>
        </section>
        <section class="section section-contact">
          <h2 class="section-title">联系方式</h2>
          <div class="section-body">
            <ul class="item-list">
              <li>手机：{{r.contact.phone}} (微信)</li>
              <li>邮箱：<a :href="'mailto:'+r.contact.email">{{r.contact.email}}</a></li>
              <li>博客：<a href="http://www.huangwenchao.com.cn">http://www.huangwenchao.com.cn</a></li>
              <li>GitHub：<a href="https://github.com/fish-ball">fish-ball</a></li>
              <li>StackOverflow：</li>
              <li>
                <!--<a href="https://stackoverflow.com/users/2544762/alfred-huang">Alfred Huang</a>-->
                <a href="https://stackoverflow.com/users/2544762/alfred-huang">
                  <img src="https://stackoverflow.com/users/flair/2544762.png?theme=clean" width="208" height="58"
                       alt="profile for Alfred Huang at Stack Overflow, Q&amp;A for professional and enthusiast programmers"
                       title="profile for Alfred Huang at Stack Overflow, Q&amp;A for professional and enthusiast programmers">
                </a>
              </li>
              <li>扫码加微信：</li>
              <li><img width="120" src="@/assets/images/wechat.jpg" /></li>
            </ul>
          </div>
        </section>
        <section class="section section-status">
          <h2 class="section-title">目前状态</h2>
          <div class="section-body">
            <ul class="item-list">
              <li>家庭状态：<br />· 已婚，有两个孩子</li>
              <li>职业状态：<br />· 目前处于自由职业者状态，对有良好发展机遇的平台及契合个人属性的岗位感兴趣。</li>
              <li>期望工作地点：<br />· 佛山/广州</li>
              <li>期望月薪：<br />· 45000 (RMB)</li>
            </ul>
          </div>
        </section>
        <section class="section section-qrcode">
          <h2 class="section-title">扫码打开简历</h2>
          <div class="section-body">
            <p><img :src="qrcode" /></p>
            <p>{{location.href}}</p>
          </div>
        </section>
      </div>
    </div>
    <div class="main-content">
      <div class="block block-education">
        <h2 class="block-title">
          <span>教育背景</span>
        </h2>
        <section class="section">
          <h3 class="section-title">
            <span class="duration">2005年 - 2009年</span>
            <span class="place">郑州大学 - 物理工程学院</span>
          </h3>
          <div class="section-body">
            <p>本科阶段学习电子科学与技术专业，获得工学学士学位。</p>
            <p>在校期间成绩优异，获得2007年全国数学竞赛全国一等奖、2008年全国数学竞赛河南省一等奖、<!--
            --> 2008-2009年第一、第二届河南省大学生编程竞赛冠军队、2008年ACM/ICPC大学生编程竞赛亚洲<!--
            --> 合肥赛区铜奖、2009年百度之星编程竞赛全国决赛（全国前50名）。</p>
          </div>
        </section>
        <section class="section">
          <h3 class="section-title">
            <span class="duration">2010年 - 2012年</span>
            <span class="place">华南理工大学 - 金融学在职研究生</span>
          </h3>
          <div class="section-body">
            <p>参加工作早期在银行任职期间，于华南理工大学修读金融学专业，修满所有学分，获得结业证书。</p>
            <p>期间学习了《微观经济学》、《宏观经济学》、《投资学》、《财务管理基础》、《货币金融学》<!--
            --> 等经济学基础课程，积累了相关方面的基础知识与技能。</p>
            <p>同期还考试通过了证券从业考试（四个科目）、银行从业资格考试（两个科目）以及会计从业资格考试，<!--
            --> 以及全国计算机技术与软件专业技术资格（水平）考试的《软件设计师》（中级）与《系统分析师》（高级）证书。</p>
          </div>
        </section>
      </div>
      <div class="block block-work-experience">
        <h2 class="block-title">
          <span>工作经历</span>
        </h2>
        <section class="section">
          <h3 class="section-title">
            <span class="duration">2009年 - 2011年</span>
            <span class="place">广发银行佛山分行 信息技术部 - 软件工程师</span>
          </h3>
          <div class="section-body">
            <p>在公司主要负责软件开发、数据分发平台运维、业务数据提取、并轮岗参与了一段时间的网络运维。</p>
            <p>任职期间参与了分行的《绩效管理系统》、《客户管理系统》部分功能开发；独立开发了《自助设备网络监控程序》与
              《NCR自助设备日志分析系统》。</p>
            <p>期间主要使用技术为微软 Visual Studio 系列：ASP.NET, C#, SQL Server 等，
              因为长期负责为业务部门完成数据提取需求（复杂的查询）以及数据分发平台的运维（日常备份、灾备切换演练等），
              积累了丰富的 SQL 使用经验。</p>
          </div>
        </section>
        <section class="section">
          <h3 class="section-title">
            <span class="duration">2011年 - 2014年</span>
            <span class="place">东莞银行佛山分行 综合管理部 - 科技专管员</span>
          </h3>
          <div class="section-body">
            <p>本人于筹办期间（开业前两个月）加入，独自一人负责了分行内部的所有信息科技相关工作，主要包括：
              设备安装、内部系统开发、信息技术工作对接（监管机构及总行科技部）。</p>
            <p>软件开发方面，独立开发了分行的《绩效管理系统》、《业务费用管理系统》与《贷款审批系统》，
              均在分行日常运营中发挥重要作用。</p>
            <p>任职期间全程参与了分行的薪酬与业务绩效体系的设计与实施，以及南海支行筹办到开业的全程支持。</p>
            <p>这个阶段除了前期使用微软技术栈进行开发，后期转为主要使用 php/mysql 的技术进行开发，
              并且开始学习使用更多新的开发技术(Node.js/Python/Android)等。</p>
          </div>
        </section>
        <section class="section">
          <h3 class="section-title">
            <span class="duration">2014年 - 至今</span>
            <span class="place">佛山市逸云计算机科技有限公司 - 自主创业/自由职业者</span>
          </h3>
          <div class="section-body">
            <p>2014年初辞职，与一名合伙人开办了公司，前期主要以开发钢结构行业的ERP为主营业务，
              一年后转型为从事软件外包开发为主，期间逐步熟悉了市场上的互联网软件开发相关的流程、技术与管理，
              并逐步扩大团队，期间一直保持以技术总监的角色主持开发并发展出一整套的开发模式与基础框架。</p>
            <p>在2018年前的这段时间带领团队完成了50个以上的大小不一的外包项目，涉及面广，涵盖了ERP系统开发、网站开发、SEO、
              系统部署运维(包括邮箱、存储、直播等各类特殊的应用服务)、移动应用开发、微信公众平台、网页爬虫等等，
              对各个环节的技术要点都基本亲手实践过。</p>
            <p>后于2017年因为业务发展方向考量，缩减了团队人员，携余下团队加入了鑫际物联网公司接手主导安全校园项目，
              最终因为项目结束，解散了团队，仅保留自己和另一位合伙人。</p>
            <p>2018年开始转为自由职业者状态，独立拓展业务，期间完成了《悍高云商》、《德富塑料网》、《中艺星光杯》
              比赛平台以及《美林轮胎销售管理系统》等项目。</p>
            <p>这段时间使用过市面上大部分的主流技术，沉淀下来的主要使用的开发框架为 Python(Django REST Framework)、
              Vue、Cordova、Flutter，部署架构采用 Openresty(Nginx)、Docker 容器化部署等，根据项目实际情况会实施 MQ、
              NoSQL等特殊的架构。</p>
          </div>
        </section>
      </div>
      <div class="block block-skills">
        <h2 class="block-title">
          <span>技术栈</span>
        </h2>
        <section class="section">
          <h3 class="section-title">
            <span class="place">前端技术：</span>
            <span class="duration">扎实的HTTP基础、熟悉H5/WEB相关标准</span>
          </h3>
          <div class="section-body">
            <ul class="skill-list">
              <li>
                <span class="tag">javascript/ES6/TypeScript</span>
                <skill-bar level="a"></skill-bar>
                <p>熟练使用 ESLint/Promise/async 等高级语法</p>
              </li>
              <li>
                <span class="tag">CSS3/Less/SASS：</span>
                <skill-bar level="a"></skill-bar>
                <p>熟悉HTML布局，能够熟练使用 CSS 高效完成 WEB 界面编写</p>
              </li>
              <li>
                <span class="tag">VueJS/NuxtJS：</span>
                <skill-bar level="a"></skill-bar>
                <p>熟练使用 VueJS 绝大部分特性，已经累积相当多的工具脚手架，例如：<a href="https://github.com/easecloud/vue-admin">vue-admin</a>，
                  但是对于 React/AngularJS 体系没有太多经验。</p>
                <p>掌握使用 NuxtJS 实现 SSR 服务器端渲染模式的开发部署。</p>
              </li>
              <li>
                <span class="tag">PhoneGap/Cordova：</span>
                <skill-bar level="a"></skill-bar>
                <p>熟练使用 Cordova 封装 HTML5 项目，而且具备 Cordova 插件开发能力，可以实现原生插件接入 Cordova 项目。</p>
              </li>
              <li>
                <span class="tag">Android Native/Kotlin</span>
                <skill-bar level="b"></skill-bar>
                <p>掌握 Android 原生开发，但对于细节的机制并没有过多的深入研究。</p>
              </li>
              <li>
                <span class="tag">iOS Native/Swift</span>
                <skill-bar level="c"></skill-bar>
                <p>能够读懂并修改现有程序，掌握应用发布流程，但是不具备整个项目的完整开发经验。</p>
              </li>
              <li>
                <span class="tag">Webpack：</span>
                <skill-bar level="c"></skill-bar>
                <p>能够针对小型的需求参照文档手动搭建 Webpack 项目。</p>
              </li>
              <li>
                <span class="tag">Flutter</span>
                <skill-bar level="c"></skill-bar>
                <p>了解 Flutter 开发模式并搭建过学习项目，暂时没有脚手架工具积累。</p>
              </li>
              <li>
                <span class="tag">微信SDK/小程序开发</span>
                <skill-bar level="b"></skill-bar>
                <p>熟悉微信 SDK 使用，已经积累有脚手架项目：
                  <a href="https://github.com/fish-ball/wx.easecloud.cn">wx.easecloud.cn</a>，能使用 uni-app 等主流框架进行小程序开发。
                </p>
              </li>
              <li>
                <span class="tag">jQuery</span>
                <skill-bar level="a"></skill-bar>
                <p>因为有早期的 JS 开发经验，对 jQuery 使用有长期的使用经验，虽然已经很少在现有项目中使用，但维护旧项目时很有优势。</p>
              </li>
              <li>
                <span class="tag">ElectronJS</span>
                <skill-bar level="b"></skill-bar>
                <p>能够使用 ElectronJS 封装客户端应用程序。</p>
              </li>
            </ul>
          </div>
        </section>
        <section class="section">
          <h3 class="section-title">
            <span class="place">后端技术：</span>
            <span class="duration">熟悉协议 RESTful/RPC/SOAP、多种语言、框架及模式</span>
          </h3>
          <div class="section-body">
            <ul class="skill-list">
              <li>
                <span class="tag">Python/Django/Scrapy</span>
                <skill-bar level="a"></skill-bar>
                <p>主力开发框架，熟悉 Django 框架绝大部分特性，能够以极快速度开发出需要的功能并且可维护性极强，有相关的脚手架积累：
                  <a href="http://github.com/easecloud/django_base">django_base</a>。另外掌握使用 Scrapy 开发网络爬虫。</p>
              </li>
              <li>
                <span class="tag">PHP/Wordpress</span>
                <skill-bar level="a"></skill-bar>
                <p>熟练使用 PHP 语言开发，尤其熟悉 Wordpress 开发（插件/主题开发）；
                  掌握使用市面的大部分 php MVC框架（ThinkPHP/CodeIgniter/Yii/Symphony等，不过需要借助文档）</p>
              </li>
              <li>
                <span class="tag">NodeJS：</span>
                <skill-bar level="c"></skill-bar>
                <p>能够读懂及修改现有代码，或使用 NodeJS 开发小型应用或工具（使用 Websocket）。</p>
              </li>
              <li>
                <span class="tag">Java：</span>
                <skill-bar level="b"></skill-bar>
                <p>了解并用过部分主流的 Java 架构和框架，例如 J2EE, Spring, Struts, Jersey, Hibernate, MyBatis, SpringBoot 等。
                  能够读懂程序、修改代码、执行部署与维护，也有新旧 Java 项目的开发经验，但是效率并不高。</p>
              </li>
              <li>
                <span class="tag">Visual Studio/C#/ASP.NET</span>
                <skill-bar level="c"></skill-bar>
                <p>熟悉语言，有 WebForm 时代的项目开发经验，但对新兴架构了解不多。</p>
              </li>
            </ul>
          </div>
        </section>
        <section class="section">
          <h3 class="section-title">
            <span class="place">架构中间件：</span>
            <span class="duration">熟悉大部分主流 WEB 相关服务，掌握容器化部署</span>
          </h3>
          <div class="section-body">
            <ul class="skill-list">
              <li>
                <span class="tag">SQL</span>
                <skill-bar level="a"></skill-bar>
                <p>对 SQL 语法使用非常熟练，能够灵活使用索引、视图、触发器、函数、存储过程等高级特性，
                  懂得 SQL 调优、部署集群等，MySQL/PostgresSQL/SQL Server 都有较多项目经验。</p>
              </li>
              <li>
                <span class="tag">Openresty/Nginx/Apache</span>
                <skill-bar level="a"></skill-bar>
                <p>熟练使用 Nginx 配置各类 Web 入口、反向代理、负载均衡、高可用等方式；还能够通过 OpenResty 用 lua
                  脚本灵活拓展简单的功能。</p>
              </li>
              <li>
                <span class="tag">MongoDB/Redis/Memcached</span>
                <skill-bar level="b"></skill-bar>
                <p>都在实际项目中用过，遇到适当的使用场景可以灵活运用。</p>
              </li>
              <li>
                <span class="tag">Docker</span>
                <skill-bar level="a"></skill-bar>
                <p>熟练使用 Docker 的各类基本特性，掌握 Docker 镜像构建以及 Auto Build 的 DockerHub 镜像发布，
                  熟练使用 docker-compose。</p>
              </li>
              <li>
                <span class="tag">MQ/RabbitMQ</span>
                <skill-bar level="b"></skill-bar>
                <p>掌握消息队列架构原理，有相关的项目经验，能够配合 Python Celery 高效开发相关模式的应用。</p>
              </li>
            </ul>
          </div>
        </section>
        <section class="section">
          <h3 class="section-title">
            <span class="place">基础技能：</span>
            <span class="duration">以上未列出的一些额外的重要技能</span>
          </h3>
          <div class="section-body">
            <ul class="skill-list">
              <li>
                <span class="tag">Vim</span>
                <skill-bar level="b"></skill-bar>
                <p>已习惯并熟练使用 Vim 编辑文本。</p>
              </li>
              <li>
                <span class="tag">Git/SVN</span>
                <skill-bar level="a"></skill-bar>
                <p>熟练使用 Git，了解高级指令的用法，能够在文档支持下执行深入的维护：rebase 等。其他版本管理系统也能掌握使用。</p>
              </li>
              <li>
                <span class="tag">Linux/Bash</span>
                <skill-bar level="b"></skill-bar>
                <p>熟悉在服务器环境和桌面环境下使用 Linux，熟悉 CentOS/Ubuntu 为主的主流发行版，能够灵活运用 Bash 脚本编写维护脚本。</p>
              </li>
              <li>
                <span class="tag">Markdown/reStructuredText/Sphinx-doc</span>
                <skill-bar level="a"></skill-bar>
                <p>熟练使用 Markdown/RST 语言编写文档，能用 Sphinx-doc 发布文档项目，但是对 Latex 没有太多了解。</p>
              </li>
              <li>
                <span class="tag">ab/wrk</span>
                <skill-bar level="c"></skill-bar>
                <p>能够执行简单的压测任务，但是尚未掌握 LoadRunner 等一些大型的压测框架。</p>
              </li>
              <li>
                <span class="tag">Other</span>
                <skill-bar level="c"></skill-bar>
                <p>另外有些涉及自动化测试、持续集成、项目管理方面的一些技能也有所涉猎，就不一一列出了。</p>
              </li>
            </ul>
          </div>
        </section>
      </div>
      <div class="block block-work-experience">
        <h2 class="block-title">
          <span>项目案例</span>
        </h2>
        <section class="section">
          <h3 class="section-title">
            <span class="duration">ACTips.org</span>
            <span class="place">业余做的 ACM 算法比赛的综合平台</span>
          </h3>
          <div class="section-body">
            <p>工作经历中列出的案例有些由于保密或可公开展示功能有限等原因，在这里仅列举一个标志性的业余项目。
              这个项目虽然暂时仅有网站端，但是内容用到的技术和架构要点都非常充分，融合了网络爬虫、消息队列、
              Vue/SPA模式前端开发、RESTful后端开发、微信 OAuth 对接等很全面的内容，并且代码开源
              （<a href="https://github.com/actips/">https://github.com/actips/</a> ）。</p>
            <p>功能上主要是实现 ACM 参赛者日常训练的解题报告提交、做题网站的代理登录以及题目、提交结果收集整理等，
              具体可以查看网站 <a href="https://actips.org">http://actips.org</a>。</p>
          </div>
        </section>
      </div>
    </div>
  </div>
</template>

<script>
import data from '@/resume/data.yml'
import SkillBar from '@/components/SkillBar'
import QRcode from 'qrcode'

export default {
  components: { SkillBar },
  data () {
    return {
      r: data,
      qrcode: '',
    }
  },
  computed: {
    location: () => location
  },
  async mounted () {
    this.qrcode = await QRcode.toDataURL(location.href)
  }
}
</script>

<style lang="less">
@import '../libs/less-template/template-defines.less';

@color-paper: white;
@color-text: #444444;
@color-text-revered: white;
@color-primary: #253F60;
@color-secondary: #82CDD2;
@sidebar-width: 280px;

a {
  color: inherit;
}

body {
  background: #F5F5F5;
  color: @color-text;
  .container {
    background: @color-paper;
    width: 960px;
    margin: 0 auto;
    box-shadow: 0 0 8px rgba(0, 0, 0, 0.3);
    position: relative;
    &::before {
      content: "";
      position: absolute;
      left: 0;
      top: 0;
      bottom: 0;
      width: @sidebar-width;
      background: @color-primary;
    }
    .clearfix();
    .sidebar {
      position: relative;
      float: left;
      width: @sidebar-width;
      background: @color-primary;
      box-sizing: border-box;
      color: @color-text-revered;
      overflow: hidden;
      a {
        color: #CCCCCC;
      }
      .block-title {
        padding: 30px;
        position: relative;
        text-align: center;
        line-height: 2rem;
        color: @color-primary;
        &::before {
          content: "";
          display: block;
          .fill-absolute();
          top: -100px;
          left: -100px;
          right: -100px;
          .rotate(-8deg);
          background: @color-secondary;
        }
        & > * {
          position: relative;
        }
        .avatar {
          img {
            display: block;
            margin: 0 auto 15px;
            width: 150px;
            height: 150px;
            border: 2px solid white;
            box-shadow: 0 0 5px rgba(0, 0, 0, 0.3);
            .circle();
          }
        }
        .name {
          font-weight: bold;
          font-size: 24px;
          .primary {
          }
          .secondary {
            font-size: 18px;
          }
        }
        .origin {
          font-size: 18px;
          color: @color-primary;
        }
        .position {
          font-size: 18px;
          color: white;
        }
      }
      .block-introduction {
        padding: 15px;
        img {
          display: block;
          max-width: 100%;
        }
        .section {
          margin-top: 30px;
          .section-title {
            font-size: 24px;
            text-align: center;
            line-height: 3em;
          }
          .section-body {
            line-height: 1.5em;
            ul.item-list {
              padding-left: 1em;
              &.disc {
                padding-left: 2em;
                list-style-type: disc;
              }
              li {
                line-height: 1.5em;
                word-wrap: break-word;
                word-break: break-all;
                margin-bottom: 0.5em;
              }
            }
          }
        }
        .section-qrcode {
          font-size: 14px;
          text-align: center;
          img {
            display: block;
            margin: 0 auto;
          }
          p {
            word-wrap: break-word;
            word-break: break-all;
            margin-bottom: 10px;
          }
        }
      }
    }
    .main-content {
      padding: 30px;
      margin-left: @sidebar-width;
      .block {
        margin: 30px 0;
        .block-title {
          overflow: hidden;
          position: relative;
          border-left: 4px solid @color-secondary;
          padding-left: 20px;
          font-size: 22px;
          line-height: 2em;
          margin-bottom: 10px;
          background: #F5F5F5;
          & > * {
            position: relative;
          }
          &::before {
            content: "";
            position: absolute;
            display: block;
            left: -50px;
            top: -50px;
            bottom: -50px;
            width: 180px;
            background: @color-secondary;
            .rotate(-8deg);
          }
        }
        .section {
          padding: 20px 10px;
          border-bottom: 1px solid #CCCCCC;
          .section-title {
            font-size: 18px;
            line-height: 1.2em;
            margin-bottom: 10px;
            .duration {
              color: @color-primary;
              margin-right: 1em;
            }
            .place {
              font-weight: bold;
              margin-right: 1em;
            }
          }
          .section-body {
            font-size: 16px;
            line-height: 1.5em;
            p {
              text-indent: 2em;
              margin-bottom: 5px;
            }
            ul.skill-list {
              font-size: 14px;
              line-height: 24px;
              li {
                color: #777;
                .tag {
                  color: darken(@color-secondary, 10%);
                  font-weight: bold;
                }
              }
            }
          }
        }
      }
    }
  }
}
</style>
