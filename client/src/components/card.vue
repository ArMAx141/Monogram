<template>
  <div class="card-container">
    <img src="../assets/img/lake-rainy.webp" alt="" class="image" />
    <div class="container">
      <h2>Heading</h2>
      <span>date</span>
      <p class="description">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptas minus optio neque
        provident recusandae eos explicabo ducimus pariatur velit? Dolor omnis nobis asperiores
        ipsam. Consectetur harum officia laborum, laboriosam nostrum quaerat illo placeat hic,
        corrupti perspiciatis distinctio atque adipisci facilis asperiores sapiente! Est architecto
        atque beatae sequi ipsum totam rem, nobis similique ratione recusandae magnam excepturi sint
        consequatur expedita impedit delectus amet fugiat corporis aliquam minus voluptates?
        Doloribus est amet optio, iusto dicta exercitationem aut, enim quae commodi porro mollitia
        debitis eligendi voluptatum! Ipsam tenetur quidem obcaecati excepturi eligendi
        exercitationem iste quas nihil. Saepe ea sapiente vitae porro quidem ullam. Ullam soluta
        unde similique, itaque error quas totam animi, eum ratione facilis accusantium saepe iste
        suscipit deserunt doloremque. Aspernatur, rem cumque numquam repudiandae architecto nostrum,
        autem modi qui officiis vitae illo velit quibusdam, impedit id odit nobis? Facere, id
        asperiores rerum odit sunt tempora, eligendi, reiciendis accusantium fuga officia ducimus?
        Dolorum, ad? Delectus nemo quas architecto deserunt eligendi consequuntur, cum, nulla
        consequatur dolor eum hic libero eveniet tempora? Magnam, minima nemo. Veniam esse possimus
        deserunt molestiae? Magni, nostrum! Doloribus sapiente facilis blanditiis laboriosam
        tempore, quisquam ratione eius maiores assumenda rem quod? Fugit ullam ipsum provident
        sapiente libero cumque quas sint.
      </p>
      <span class="read-more">Read more...</span>
    </div>
  </div>
</template>

<script setup lang="ts"></script>

<style scoped>
.card-container {
  background-color: wheat;
  padding: 1rem;

  display: flex;
  gap: 1rem;
}

.image {
  object-fit: cover;
  width: 230px;
  height: 230px;
}

.container {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}

.description {
  overflow: hidden;

  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-line-clamp: 4;
  line-clamp: 4;
}
</style>
