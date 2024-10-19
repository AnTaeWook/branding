<script>
import Header from "./Header.svelte";
import Footer from "./Footer.svelte";
import {getNews} from "../../assets/news.js";

export let params = {};
const article = getNews(parseInt(params.id));
</script>

<Header/>
<main class="container">
  <div class="main-header">
    <h2>{article.title}</h2>
    <p class="class date">{article.date}</p>
    <img src={article.detailImgUrl} alt={article.title}/>
  </div>
  <article>
    {@html article.desc}
  </article>
</main>
<Footer/>

<style lang="scss">
  .main-header {
    h2 {
      margin-bottom: 10px;
    }
    .date {
      margin-bottom: 20px;
      font-size: 15px;
      color: #666;
    }
  }

  article {
    margin-top: 50px;
  }

  .container {
    background: #fff;
  }
</style>