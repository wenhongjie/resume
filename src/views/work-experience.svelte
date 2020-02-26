<script>
  import Card from "components/card";
  import Title from "components/title";
  import SubTitle from "components/title/sub-title";

  const list = [
    {
      title: "苏州嘉展科技有限公司 前端工程师(2019.3 ~ 现在), 主要负责不同项目的启动, 协助需求, 开发项目组件, 业务开发, 前端架构演进, 带领和给新人培训.",
      children: [
        {
          title: "甄喜月国际月子会所管理系统, 手机端和PC端, 该系统使用Vue全家桶, 总共4个前端(2个新人), 我主要负责框架搭建和提供组件, 比如护理时间线组件, " + 
          '弹框组件, 日历组件(疾病追踪和排程), 分页选择器, Element组件二次封装, 上传组件, 打印组件...该项目进行了大量的优化.性能上, 最大单文件仅有50kb左右, 无缓存首屏进入耗时仅仅' + 
          '1.4s, 静态资源服务器使用nginx并且在gzip质量和效率上达成了平衡, 远程下拉菜单选择器采用分页的形式, 以避免消耗多余的服务器资源; 用户体验上, 表格分页页面保持了表头固定的形式(二次封装了组件可配置的), ' + 
          '增加了一些手势操作; 开发体验上, 鉴于公司大多数前端不会使用typescript 以及react全家桶, 考虑到公司的成本, 因此采用了js + typescript声明文件的形式, 加强了编辑器的' + 
          '代码提示, 同时给所开发的组件写了文档, 因此开发体验较为良好.',
          href: 'https://babycare.cloudkeeper.cn/'
        },
        {
          title: "云康糖尿病联盟微信公众号."
        },
        {
          title: "云康社区小程序, 使用React + Taro开发, 本来想借此机会推广react, 公司认为成本过高, 最后只能我一人开发完, 同时react也没推广开来."
        },
        {
          title: '智盛精密智能工厂管理系统(MES), 同样经过优化的项目, 组件更加规范.'
        },
        {
          title: '物联管家小程序.'
        }

      ]
    },
    {
      title: "苏州新启成传媒股份有限公司 高级前端工程师(2018.6 ~ 2019.3), 公司是附属部门, 前端由我全权负责, 开发主要是两个重量级产品, DSP广告平台以及看我视频网.",
      children: [
        {
          title: "看我视频网, 当时公司刚刚架构转型向前后端分离模式, 我帮助PHP团队制定restful接口规范, 自己则负责全部前端项目",
          href: 'https://www.tvcapp.com/'
        },
        {
          title: "DSP广告平台"
        }
      ]
    },
    {
      title: "苏州八零传媒 前端工程师(2017.10 ~ 2018.6).",
      children: [
        {
          title: "绿云众筹"
        },
        {
          title: "睿投, 接手项目",
          href: 'http://www.ritering.cn/'
        }
      ]
    }
  ];
</script>

<Card title="工作经验">
  {#each list as item}
    <Title title={item.title}>
      {#each item.children as subItem}
        {#if subItem.href}
          <SubTitle>
            <a href={subItem.href}>{subItem.title}</a>
          </SubTitle>
          {:else}
          <SubTitle>{subItem.title}</SubTitle>
        {/if}
      {/each}
    </Title>
  {/each}
</Card>
