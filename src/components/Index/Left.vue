<template>
  <div class="base-frame">
    <header class="head-frame flex-between">
      <div class="flex-col-center">
        <img class="head-icon" src="https://admore-cas.oss-cn-hangzhou.aliyuncs.com/xcx/img/index/shike_icon.png">
        <div class="head-title">应用试客 <span class="head-divide">|</span> 小程序投放平台</div>
      </div>
      <div class="head-handle flex-col-center">
        <img class="handle-icon" src="https://admore-cas.oss-cn-hangzhou.aliyuncs.com/xcx/img/index/notice.png">
        <img class="handle-icon" src="https://admore-cas.oss-cn-hangzhou.aliyuncs.com/xcx/img/index/self.png">
      </div>
    </header>
    <div class="flex">
      <nav class="left-nav">
        <ul class="nav-list">
          <li class="nav-item cur">
            <img class="item-icon" src="https://admore-cas.oss-cn-hangzhou.aliyuncs.com/xcx/img/index/mnp_cur.png">
            <!-- <img class="item-icon" src="https://admore-cas.oss-cn-hangzhou.aliyuncs.com/xcx/img/index/mnp.png"> -->
            <span class="item-title">程序管理</span>
          </li>
          <li class="nav-item">
            <img class="item-icon" src="https://admore-cas.oss-cn-hangzhou.aliyuncs.com/xcx/img/index/spread.png">
            <span class="item-title">数据分析</span>
          </li>
          <li class="nav-item">
            <img class="item-icon" src="https://admore-cas.oss-cn-hangzhou.aliyuncs.com/xcx/img/index/doc.png">
            <span class="item-title">对接文档</span>
          </li>
          <li class="nav-item">
            <img class="item-icon" src="https://admore-cas.oss-cn-hangzhou.aliyuncs.com/xcx/img/index/account.png">
            <span class="item-title">账户管理</span>
          </li>
          <li class="nav-item">
            <img class="item-icon" src="https://admore-cas.oss-cn-hangzhou.aliyuncs.com/xcx/img/index/shike.png">
            <span class="item-title">体验试客</span>
          </li>
        </ul>
      </nav>
      <article class="main-content">
        <div class="main-title">小程序管理</div>
        <div class="main-tab">
          <ul class="tab-list">
            <li class="tab-item cur">程序管理</li>
            <li class="tab-item">程序广场</li>
          </ul>
        </div>
        <div class="main-list">
          <div class="flex-between">
            <div class="list-title">我的小程序</div>
            <div class="list-add-btn">添加</div>
          </div>
          <table class="table margin-top-5">
            <thead>
              <tr>
                <th>ID</th>
                <th>名称</th>
                <th>标签</th>
                <th>标语</th>
                <th>二维码</th>
                <th>封面</th>
                <th>截图</th>
                <th>操作</th>
              </tr>
            </thead>
            <tbody class="program">
              <tr>
                <td>0001</td>
                <td>
                  <img class="icon" src="http://admore-cas.oss-cn-hangzhou.aliyuncs.com/xcx/img/test/icon.png" />
                  <div>
                    小程序A
                  </div>
                </td>
                <td>工具</td>
                <td>这里最多显示十二字的内容</td>
                <td><img class="code" src="http://admore-cas.oss-cn-hangzhou.aliyuncs.com/xcx/img/test/icon.png" /></td>
                <td>
                  <img class="code" src="http://admore-cas.oss-cn-hangzhou.aliyuncs.com/xcx/img/test/icon.png" />
                </td>
                <td>
                  <img class="screenshot" src="http://admore-cas.oss-cn-hangzhou.aliyuncs.com/xcx/img/test/icon.png" />
                </td>
                <td>
                  <a>对接</a>
                </td>
              </tr>
            </tbody>
          </table>
        </div>
      </article>
    </div>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        msg: "Welcome"
      };
    },
    created() {}
  };
</script>

<style lang="less">
  .base-frame {
    width: 100%;
    height: 100%;
    margin: 0;
    padding: 0;
    background-color: #f7f8fa;
    text-align: left;
    font-style: normal;
    font-stretch: normal;
    line-height: normal;
    letter-spacing: normal;
    color: #000000;
    font-weight: 300;
    .head-frame {
      height: 1rem;
      padding: 0 0.5rem;
      background-color: #ffffff;
      box-shadow: 0 0.01rem 0.05rem 0 rgba(159, 159, 159, 0.5);
      .head-icon {
        width: 0.68rem;
        height: 0.66rem;
        margin-right: 0.43rem;
      }
      .head-title {
        display: flex;
        align-items: center;
        font-size: 0.4rem;
        .head-divide {
          margin: 0 0.3rem;
        }
      }
      .head-handle {
        position: relative;
        right: 0;
        .handle-icon {
          width: 0.32rem;
          height: 0.32rem;
          margin-left: 0.34rem;
        }
      }
    }
    .left-nav {
      width: 2.8rem;
      // min-height: 8.5rem;
      padding-top: 0.03rem;
      .nav-list {
        min-height: 8rem;
        margin: 0.49rem 0 0;
        padding: 0;
        border-right: solid 0.01rem #979797;
        .nav-item {
          display: flex;
          justify-content: center;
          align-items: center;
          padding: 0.25rem 0;
          .item-icon {
            width: 0.45rem;
            height: 0.45rem;
            margin-right: 0.38rem;
          }
          .item-title {
            font-size: 0.25rem;
          }
        }
        .nav-item.cur {
          color: #2ab228;
          border-left: solid 0.09rem #1bad19;
        }
      }
    }
    .main-content {
      margin: 0.5rem 0.5rem 0;
      flex-grow: 1;
      .main-title {
        font-size: 0.44rem;
        color: #3a3a3a;
      }
      .main-tab {
        border-bottom: solid 0.02rem #ebebef;
        .tab-list {
          display: flex;
          margin-top: 0.2rem;
          font-size: 0.26rem;
          color: #323232;
          .tab-item {
            display: flex;
            justify-content: center;
            align-items: center;
            width: 1.74rem;
            height: 0.6rem;
            color: #9f9f9f;
          }
          .tab-item.cur {
            border-bottom: 0.03rem #1bad19 solid;
            color: #323232;
          }
        }
      }
      .main-list {
        min-height: 2.5rem;
        margin-top: 0.3rem;
        padding: 0.32rem 0.45rem;
        border-radius: 0.06rem;
        background-color: #fff;
        box-shadow: 0 0.01rem 0.04rem 0 rgba(80, 80, 80, 0.21);
        .list-title {
          font-size: 0.33rem;
          color: #353535;
        }
        .list-add-btn {
          width: 1.69rem;
          height: 0.52rem;
          display: flex;
          justify-content: center;
          align-items: center;
          border-radius: 0.04rem;
          background-color: #18ac17;
          font-size: 0.23rem;
          color: #fff;
        }
        .program{
            .icon{
              width: .56rem;
              height: .56rem;
              border-radius:0.1rem;
            }
            .code{
              width: .88rem;
              height: .88rem;
              border-radius:0.1rem;
            }
            .screenshot{width: .88rem;}
          }
      }
    }
  }
</style>
