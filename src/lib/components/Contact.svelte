<script>
  import Header from "./Header.svelte";
  import Footer from "./Footer.svelte";
</script>

<Header/>
<main class="container">
  <h2>최고의 무대를 선사하겠습니다.</h2>
  <div class="contact">
    <figure class="map">
      <!-- svelte-ignore a11y-missing-attribute -->
      <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3174.398327003768!2d127.05364987642092!3d37.28569234018148!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x357b5b1fea3daa91%3A0xecf3d8c186d80c6!2z6rSR6rWQ7IS87Yq465-07ZG466W07KeA7Jik7Iuc7YuwIOyYpO2UvOyKpO2FlA!5e0!3m2!1sko!2skr!4v1729347446325!5m2!1sko!2skr" width="100%" height="450" style="border:0;" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
    </figure>
    <address>
      <p>경기도 수원시 영통구 도청로 10 4층<br>광교 센트럴 푸르지오시티</p>
      <p>Email:
        <a href="mailto:antk7894@gmail.com">antk7894@gmail.com</a></p>
      <p>Tel:
        <a href="tel:031-000-0000">031-000-0000</a> /
        <a href="tel:010-000-0000">010-000-0000</a>
      </p>
      <p>Fax: 031-000-0000</p>
    </address>
  </div>
</main>
<Footer/>

<style lang="scss">
  .contact {
    display: flex;
    gap: 75px;
    figure, address {
      width: 50%;
    }

    address {
      font-style: normal;
    }
    a {
      color: inherit;
    }
  }

  .container {
    background: #fff;
  }
</style>