<script>
  import Card from "components/card";
  import Achievement1 from 'images/achieve01.png'
  import Achievement2 from 'images/achieve02.png'
</script>

<Card title="荣誉和成就">
  <a href={Achievement1} target="_blank"><img class="img" src={Achievement1} alt="荣誉"></a>
  <a href={Achievement2} target="_blank"><img class="img" src={Achievement2} alt="荣誉"></a>
</Card>    

<style>
.img {
  width: 45%;
  min-width: 135px;
  height: auto;
}
</style>
