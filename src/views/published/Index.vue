<template>
  <section class="published">
    <div class="published__heading">
      <img src="/images/top_logo.png" alt="ロゴ画像：テイクアウトとデリバリー情報" class="position_image" />
      <h2 class="heading">みんなでつくる！新宿区テイクアウト・デリバリー情報</h2>
    </div>
    <div class="published__text">
      <p>
        SHINJUKU
        EATS（eats.codeforshinjuku.org）では、店舗、そして新宿区内の飲食店を愛するみなさまから飲食店情報を募集しております。
        <br />情報提供フォームより投稿をお願いいたします。
        <br />情報が重複する場合には店舗からの情報提供を優先し、事務局で掲載内容の調整を行います。
      </p>

      <h3>画像の登録について</h3>

      <p>
        画像は1点掲載可能です。横幅：900px、高さ：600pxでご用意いただくときれいに表示できます。
        <br />テイクアウトメニューや店舗の画像などをご用意の上、ダウンロード可能なURLをフォームに入力いただくか、次の宛先にメールで送付してください。
        <br />画像送付先メールアドレス：codeforshinjuku@gmail.com
      </p>

      <h3>登録情報の取り扱いについて</h3>
      <p>
        登録情報は写真も含めてオープンデーターとして公開されます。
        <br />第三者による自由な利用を無条件で許可できる内容のみとしてください。
      </p>
      <p>登録情報に不備がある場合、新宿区内に事業の実態がない場合、取得している営業許可の範囲をこえるメニュー（提供できないメニュー）や、公序良俗に反する記述などがある場合には、予告なく内容修正、掲載見送り、削除を行う場合があります。</p>
    </div>
    <a href="#" target="_blank" title="情報提供フォームを新規ウィンドウで開きます" class="square_button">情報提供フォーム</a>
  </section>
</template>

<script>
export default {
  name: "Index"
};
</script>

<style scoped lang="scss">
@import "@/assets/scss/style.scss";
.published {
  position: relative;
  width: 50%;
  margin: 0 auto;
  &__heading {
    position: relative;
    z-index: 20;
    width: 52%;
    margin: 0 auto 5.3rem;
    .position_image {
      margin: 0 0 7.1rem;
    }
    .heading {
      font-size: 2.4rem;
      text-align: center;
    }
  }
  &__text {
    margin: 0 0 5.2rem;
    &__heading {
      text-align: center;
      font-size: 2rem;
      margin: 8rem auto 4rem auto;
    }
    &__description {
      text-align: center;
    }
    &__bnrs {
      list-style-type: none;
      margin: 2rem 0;
      padding: 0;
      li {
        display: inline-block;
        padding: 0 1rem;
        width: 20%;
        height: auto;
      }
    }
  }
  h3 {
    margin: 4rem 0 2rem 0;
  }
  .square_button {
    display: block;
    width: 35%;
    min-width: 34.5rem;
    font-size: 1.8rem;
    color: $mainColor;
    margin: 0 auto 2rem auto;
    line-height: 6rem;
    text-align: center;
    border: 0.1rem solid $mainColor;
  }
  @include mediaMobile {
    width: 100%;
    padding: 0 1.5rem;
    &__heading {
      width: 61.8%;
      margin: 0 auto 4.1rem;
      .position_image {
        margin: 0 0 2.9rem;
      }
      .heading {
        font-size: 1.8rem;
      }
    }
    .square_button {
      width: 100%;
      min-width: initial;
      font-size: 1.4rem;
      line-height: 4rem;
    }
  }
  @include mediaTablet {
    padding: 0 0 3rem;
    &__heading {
      width: 70%;
      .position_image {
        margin: 0 0 2.9rem;
      }
    }
  }
  @include mediaPc {
    min-width: 96rem;
  }
}
</style>
