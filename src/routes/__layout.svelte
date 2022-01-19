<script>
  import Title from "$lib/title.svelte";
  import Footer from "$lib/year.svelte";
  import "../styles/global.css";
</script>

<div class="wrapper">
  <div class="header">
    <div class="title">
      <Title />
    </div>
  </div>

  <div class="main"><slot /></div>

  <div class="footer">
    <Footer />
  </div>
</div>

<style>
  .wrapper {
    height: 100vh;
    display: flex;
    flex-direction: column;
  }
  .header {
    background: rgba(0, 0, 0, 0.1);
  }
  .main {
    max-width: 1920px;
    flex: 1;
    overflow: auto;
  }
  .title {
    display: flex;
    align-items: center;
    margin-right: 20px;
  }
  .footer {
    background: rgba(0, 0, 0, 0.1);
  }
</style>
