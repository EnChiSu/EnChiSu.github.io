---
title: Utterances setup for the Hexo Minos Theme
---
網路上已經有很多Hexo主題設置相關的文章，本篇介紹如何為Minos主題設置utterances留言區。

### 安裝
1. 在Github創建一個Repository，設為public
2. 安裝[utterances app](https://github.com/apps/utterances) (選`Only select repositories`使用步驟一的那個repo)
<p align="center">
  <img src="/images/utterances-install-modal.jpg" width=512 />
</p>

3. 輸入 owner/repo，即要放留言的Github倉庫名稱
4. 設定 issue 標題的開法
5. 選擇 comment 區的主題樣式
6. 在`\themes\minos\layout\comment`底下新增一個utterances.ejs檔案，將自動產生的程式碼貼進這個檔案裡
<p align="center">
  <img src="/images/utterances-setup.png" width=600 />
</p>
7. 在`\themes\minos\_config.yml`裡的comment區塊填上utterances，如下
``` bash
# Comment plugin settings.
comment:
  type: utterances
  shortname:
```

### References
https://annkuoq.github.io/blog/2020-03-09-add-utterances-comment-widget-to-hexo/
