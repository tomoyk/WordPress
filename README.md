# WordPressのソースを読んでみる

## index.php

- 定数`WP_USE_THEMES`を宣言している。
- `wp-blog-header.php`を読み込んでいる。ここで`require_once`ではなく`require`が使われているのが気になる。

**基本的にこのファイルでは何かしているわけではなく、あくまで呼び出しだけのよう。**

