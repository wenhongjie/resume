<script>
import avatar from 'images/avatar.jpg'
</script>

<header class="header">
  <img class="avatar" src={avatar} alt="avatar">
  <section class="info">
    <h2>温宏杰</h2>
    <p>高级前端开发工程师</p>
  </section>
</header>

<style>

.header {
  --size: 80px;
  padding: 4px;
  margin-bottom: 8px;
  border-bottom: 1px solid var(--primary-color);
}

.avatar, .info {
  vertical-align: middle;
}

.avatar {
  width: var(--size);
  height: var(--size);
  border-radius: 50%;
}

.info {
  display: inline-block;
  margin-left: 20px;
}

p {
  color: #999;
}
</style>