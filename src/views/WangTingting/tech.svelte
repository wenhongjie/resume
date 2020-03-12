<script>
  import Card from "components/card";
  import Title from "components/title";
  import SubTitle from "components/title/sub-title";

  const techList = [
    {
      title: "工具",
      children: [
        "UClient, 用于财务结算工作.",
        "Au, 处理音频信息."
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
