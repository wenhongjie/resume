<script>
  import "styles/app.css";
  import Effect from "components/effect";
  import Header from "./header";
  import Contact from "./contact";
  import Education from "./education";
  import Tech from "./tech";
  import WorkExperience from "./work-experience";
  import Achievement from "./Achievement";
  import Specialty from "./specialty";
  import Hobby from "./hobby";
  import Other from "./other";
</script>

<style>
  .main {
    width: 100%;
    height: 100%;
    padding: 8px;
    max-width: 800px;
    margin: 0 auto;
    overflow: auto;
    background: var(--main-background-color);
  }
</style>

<Effect />
<main class="main">
  <!-- 头信息 -->
  <Header />

  <!-- 联系方式 -->
  <Contact />

  <!-- 教育 -->
  <Education />

  <!-- 技术 -->
  <Tech />

  <!-- 工作经验 -->
  <WorkExperience />

  <!-- 特长 -->
  <Specialty />

  <!-- 荣誉和成就 -->
  <Achievement />

  <!-- 兴趣和爱好 -->
  <Hobby />

  <!-- 其他 -->
  <Other />
</main>
