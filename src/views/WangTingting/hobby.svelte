<script>
  import Card from "components/card";
  import Title from "components/title";
  import SubTitle from "components/title/sub-title";

  const list = [
    { title: "电影" },
    { title: "古风" },
    { title: "旅游" },
    { title: "音乐" }
  ];
</script>

<Card title="兴趣爱好">
  {#each list as item}
    <Title title={item.title} />
  {/each}
</Card>
