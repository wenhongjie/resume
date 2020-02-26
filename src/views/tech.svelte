<script>
  import Card from "components/card";
  import Title from "components/title";
  import SubTitle from "components/title/sub-title";

  const techList = [
    {
      title: "基础技术",
      children: [
        "ECMASCRIPT, 研究过多个库和框架的源码(axios,nodejs, jquery, vue, lodash), 写过一些工具库(webpack-progress-bar, fe-utils, qc-players).",
        "CSS及CSS预处理器(css-next, sass, less, stylus).",
        "H5及DOM"
      ]
    },
    {
      title: "工具",
      children: ["Git, VSCode, SS, 境外服务器.", "LeetCode."]
    },
    {
      title: "扩展",
      children: [
        "Typescript, 使用Typescript可以避免大量的错误(90%以上), 同时能够增强代码的可读性, 因此ts是新生代的前端er的利器.",
        "CSS及CSS预处理器(css-next, sass, less, stylus).",
        "Nodejs, nodejs相比JavaScript拥有和操作系统交互的权限,因此可以获得socket编程, 文件系统api等一些浏览" +
          "器中无法实现的功能,因此可以做更多的事情,可以开发命令行工具, 可以开发Web服务端, 可以做爬虫, 可以做桌面应用.",
        "Dart, dart是一个现代语言, 不失JS的灵活, 兼具Java的安全, 它的思想汲取了那些著名语言好的部分.",
        "Nginx, 如果你有一个自己的服务器, 如果你想开发一个属于自己的网站, 如果你想把这个网站部署到你的服务器上, " +
          "那么nginx是有必要学习一下的, 只需要了解它的核心模块, 你就可以游刃有余地部署你的项目."
      ]
    },
    {
      title: "框架",
      children: [
        "Vue, 写过N个Vue组件, 大量运用在管理系统中, 读过源码.",
        "React, 灵活的框架,与TypeScript结合开发大型项目游刃有余.",
        "Electron, 如果你的前端应用无法满足于一些权限, 比如获取本机MAC地址,读取本机文件,那么可以用Electron来开发一款跨平台的桌面应用.",
        "Nestjs, 由TypeScript和Nodejs和webpack结合带来的服务端框架,被称为node中的spring boot.",
        "Flutter, 这是一个全新的移动端开发框架, 开发语言为dart, 国外和国内的巨头正在狂热地使用它.",
        "Svelte, 这个是开发rollup.js的作者开发的前端框架, 本页面就使用的这个框架, 如果写一些相对较小的项目或者demo, 使用它是不二的选择, 几乎为" +
          "0的runtime和高效的性能(据vue的作者尤雨溪说简单的项目性能和vanillajs差不多)."
      ]
    }
  ];
</script>

<Card title="职业技能">
  {#each techList as item, index}
    <Title title={item.title}>
      {#each item.children as title, subIndex}
        <SubTitle index={subIndex + 1}>{title}</SubTitle>
      {/each}
    </Title>
  {/each}
</Card>
