<script>
  import Card from "components/card";
  import Title from "components/title";
  import SubTitle from "components/title/sub-title";

  const list = [
    {
      title: "尚层装饰(北京)有限公司苏州分公司 结算专员(2018.10 ~ 现在), 主要负责财务结算, 凭证导入, 对账.",
      children: [
        {
          title: "结算效率高, 对待客户和公司内部人员及其有礼貌."
        }
      ]
    },
    
    {
      title: "苏州迪杨信息科技有限公司 数据处理专员(2018.3 ~ 2018.10) 主要负责数据处理工作.",
      children: []
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
