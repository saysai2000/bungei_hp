<template>
  <div>
    <v-row>
      <v-col cols="12">
        <v-card>
          <v-tabs>
            <v-tab>活動理念</v-tab>
            <v-tab>ご挨拶</v-tab>
            <v-tab>活動情報</v-tab>
            <v-tab>メンバー</v-tab>
            <v-tab>歴史</v-tab>
            <v-tab>パートナー</v-tab>
          </v-tabs>
        </v-card>
      </v-col>
    </v-row>
    <v-row>
      <v-carousel>
        <v-carousel-item
          v-for="(item,i) in items"
          :key="i"
          :src="item.src"
          reverse-transition="fade-transition"
          transition="fade-transition"
        ></v-carousel-item>
      </v-carousel>
    </v-row>
    <v-row>
      <v-col cols="4">
        <img src="https://pbs.twimg.com/media/EfM8Od0VoAgL-xZ.jpg:medium" alt="butyou" width="360" height="358" />
      </v-col>
      <v-col cols="8">
        どうもこんにちわ。<br />部長の池牛です。皆さんも文芸部で頑張ってみましょう！<br/>私は神です。一緒に世界を滅ぼしましょう。
      </v-col>
    </v-row>
    <v-row>
      <v-col cols="8">
        <dl class="cf">
          <dt>2021年11月15日(月)</dt>
            <dd>
              <a href="違うURL">タイトル</a>
            </dd>
          <dt>2021年11月15日(月)</dt>
            <dd>
              <a href="違うURL">タイトル</a>
            </dd>
          <dt>2021年11月08日(月)</dt>
            <dd>
              <a href="違うURL">タイトル</a>
            </dd>
          <dt>2021年11月05日(金)</dt>
            <dd> 
              <a href="違うURL">タイトル</a>
            </dd>
          <dt>2021年10月29日(金)</dt>
            <dd>
              <a href="違うURL">タイトル</a>
            </dd>
          <dt>2021年10月29日(金)</dt>
            <dd>
              <a href="違うURL">タイトル</a>
            </dd>
          <dt>2021年10月20日(水)</dt>
            <dd>
              <a href="違うURL">タイトル</a>
            </dd>
        </dl>
        </v-col>
      <v-col cols="4">
        <a class="twitter-timeline" data-lang="ja" data-width="400" data-height="600" data-theme="light" href="https://twitter.com/momobungei?ref_src=twsrc%5Etfw">Tweets by momobungei</a>
          <script async src="https://platform.twitter.com/widgets.js" charset="utf-8">
          </script>
      </v-col>
    </v-row>
  </div>
</template>

<script>
  export default {
    data () {
      return {
        items: [
          {
            src: 'https://domani.shogakukan.co.jp/wp-content/uploads/2020/11/shutterstock_1491910001_790x500.jpg',
          },
          {
            src: 'https://mag.japaaan.com/wp-content/uploads/2021/02/Akutagawa.ryunosuke-1-1280x720.jpg',
          },
          {
            src: 'https://livedoor.blogimg.jp/lanovebunko/imgs/b/6/b6d0f572.jpg',
          },
          {
            src: 'https://www.pakutaso.com/shared/img/thumb/dandaIMGL9067_TP_V.jpg',
          },
          {
            src: 'https://cdn-ak.f.st-hatena.com/images/fotolife/P/PALLAGEEM/20210122/20210122235733.jpg',
          },
        ],
      }
    },
  }
</script>

