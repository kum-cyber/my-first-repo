# my-first-repo　hi bear
images/sample.jpg
<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <title>こんにちは GitHub Pages</title>
</head>
<body>
  <h1>はじめてのGitHubページ</h1>
  <p>これはテストページです。</p>
</body>
</html>
<!DOCTYPE html>
<html>
<head>
<title>ランダムタヌキ</title>
<style>
  img {
    max-width: 500px; /* 画像の最大幅を設定 */
    height: auto;
  }
</style>
</head>
<body>

<img id="tanukiImage" src="" alt="ランダムなタヌキ">
<button onclick="changeTanuki()">別のタヌキを見る</button>

<script>
  const tanukiImages = [
    "https://www.collinsdictionary.com/images/thumb/raccoondog_87452444_250.jpg?version=6.0.83",  // 例1: フリー素材サイトのURL
    "https://japannews.yomiuri.co.jp/wp-content/uploads/2023/09/10735239.jpg",  // 例2
    "https://example.com/tanuki3.gif",  // 例3
    // ... 他のタヌキ画像のURLをここに追加 ...
  ];

  const tanukiImageElement = document.getElementById("tanukiImage");

  function changeTanuki() {
    const randomIndex = Math.floor(Math.random() * tanukiImages.length);
    tanukiImageElement.src = tanukiImages[randomIndex];
  }

  // ページ読み込み時に最初のタヌキを表示
  changeTanuki();
</script>

</body>
</html>
