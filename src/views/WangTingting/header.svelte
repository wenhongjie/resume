<script>
import avatar from 'images/avatar_wangtingting.jpg'
</script>

<header class="header">
  <img class="avatar" src={avatar} alt="avatar">
  <section class="info">
    <h2>王婷婷</h2>
    <p>财务结算专员</p>
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