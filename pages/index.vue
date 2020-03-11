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
            </ul>
          </div>
        </section>
        <section class="section section-prize">
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
            </ul>
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
            <p>参加工作早期在银行任职期间，与华南理工大学修读金融学专业，修满所有学分，获得结业证书。</p>
            <p>期间学习了《微观经济学》、《宏观经济学》、《投资学》、《财务管理基础》、《货币金融学》<!--
            --> 等经济学基础课程，积累了相关方面的基础知识与技能。</p>
            <p>同一时期内还考试通过了证券从业考试（四个科目）、银行从业资格考试（两个科目）以及会计从业资格考试，<!--
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
            <p>期间全程参与了分行的薪酬与业务绩效体系的设计与实施，以及南海支行筹办到开业的全程支持。</p>
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
            <p>2014年初辞职，与一名合伙人开办了公司，前期目标主要以开发钢结构行业的ERP为主营业务，
              一年后转型为从事软件外包开发为主，期间逐步熟悉了市场上的互联网软件开发相关的流程、技术与管理，
              并逐步扩大团队，期间一直保持以技术总监的角色主导开发并发展了一整套的开发模式与基础框架。</p>
            <p>在2018年前的这段时间带领团队完成了50个以上的大小不一的外包项目，涉及面广，涵盖了ERP系统开发、网站开发、
              系统部署运维(包括邮箱、存储、直播等各类特殊的应用服务)、移动应用开发、微信公众平台等等，
              对各个环节的技术要点都基本亲手实践过。</p>
            <p>后于2017年因为业务发展方向考量，缩减了团队人员，携余下团队加入了鑫际物联网公司接手主导安全校园项目，
              最终因为项目结束，解散了团队，仅保留自己和另一位合伙人。</p>
            <p>2018年开始转为自由职业者状态，独立拓展业务，期间完成了《悍高云商》、《德富塑料网》、《中艺星光杯》
              比赛平台以及美林轮胎销售管理系统等项目。</p>
          </div>
        </section>
      </div>
    </div>
  </div>
  </div>
</template>

<script>
import data from '@/resume/data.yml'

export default {
  data () {
    console.log(data)
    return {
      r: data
    }
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
        .section {
          margin-top: 30px;
          &.section-prize {
            font-size: 16px;
          }
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
                word-wrap: break-word;
                word-break: break-all;
                margin-bottom: 0.5em;
              }
            }
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
            }
          }
          .section-body {
            font-size: 16px;
            line-height: 1.5em;
            p {
              text-indent: 2em;
              margin-bottom: 5px;
            }
          }
        }
      }
    }
  }
}
</style>
