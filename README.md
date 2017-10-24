# WordPressのソースを読んでみる

## index.php

- 定数`WP_USE_THEMES`を宣言している。
- `wp-blog-header.php`を読み込んでいる。ここで`require_once`ではなく`require`が使われているのが気になる。

**基本的にこのファイルでは何かしているわけではなく、あくまで呼び出しだけのよう。**

## wp-blog-header.php

- wp-load.phpを読み込む
- `wp()`を呼び出し
- template-loader.phpを読み込む

## wp-load.php

- `wp_fix_server_vars()`
