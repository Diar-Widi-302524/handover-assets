<script>
  import Title from "$lib/title.svelte";
  import Footer from "$lib/year.svelte";
  import "../../styles/global.css";
</script>

<div class="wrapper">
  <div class="header">
    <div class="title">
      <Title title="Handover Assets Guides" />
      <nav>
        <ul>
          <div class="option">
            <li><a href="/">Home</a></li>
            <li><a href="/about">About</a></li>
            <li><a href="/guides">Guides</a></li>
          </div>
        </ul>
      </nav>
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
  ul li {
    display: inline-block;
  }
  .option {
    margin-right: 20px;
  }
  a {
    margin-left: 20px;
  }
  .title {
    display: flex;
    align-items: center;
    justify-content: space-between;
  }
  .footer {
    background: rgba(0, 0, 0, 0.1);
  }
</style>
