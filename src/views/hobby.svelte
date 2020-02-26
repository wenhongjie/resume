<script>
  import Card from "components/card";
  import Title from "components/title";
  import SubTitle from "components/title/sub-title";

  const list = [
    { title: "天文" },
    { title: "微生物, (自备6000倍光学显微镜)" },
    { title: "金融" },
    { title: "游戏" },
    { title: "旅游" }
  ];
</script>

<Card title="兴趣爱好">
  {#each list as item}
    <Title title={item.title} />
  {/each}
</Card>
