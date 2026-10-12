# ほほえみ勤務表・タイムカード（kinmuhyo-timecard）について

合同会社発達支援ほほえみカレッジが事業所に配っている、勤務表とタイムカードを合わせたアプリです。
公開先は https://hohoemi2018.github.io/kinmuhyo-timecard/ です。

この `index.html` は直接編集しません。元ファイルは別リポジトリ `hohoemi2018/kinmuhyo` の `_src/hohoemi-src.html` にあり、
勤務表アプリ・タイムカードアプリと同じ元ファイルから `_src/build.py` で作り分けています（`const APP='both'`）。
直すときは kinmuhyo の `.claude/CLAUDE.md` の手順に従い、kinmuhyo・timecard・kinmuhyo-timecard を同じフォルダに並べて作業してください。

入力データは各事業所のブラウザの localStorage（キー `hohoemi-kinmuhyo-tc-v1`）にあります。キーは変えず、以前のデータが読めるようにしてください。
「これまでのデータを取りこむ」は、同じ端末の勤務表（`hohoemi-kinmuhyo-v1`）とタイムカード（`hohoemi-timecard-v1`）のデータを読むだけで、もとのデータは変えません。
