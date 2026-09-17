幫我把這個資料夾目前的修改 commit 起來,然後 push 到 GitHub 上。

commit 訊息你自己看修改的內容想一個講得清楚在做什麼就好,不用每次都問我。如果這個資料夾還沒有連到任何 GitHub repo(沒有設定 remote),要先跟我要這兩個東西:

- repo 的網址(例如 `https://github.com/帳號/repo名稱.git`),如果 repo 還沒建好,要先用 `gh repo create` 幫我建一個新的、獨立的 repo(每個範例專案各自一個 repo,不要塞進同一個共用的 repo 裡)
- 要 push 去哪個分支(沒特別說的話預設 main 就好)

如果已經連好 remote 了,直接 commit 完 push 上去就好,不用再確認。push 需要的 GitHub 登入是靠 Git Credential Manager(跟 `gh auth login` 是分開的兩套),第一次 push 沒登入過的話會跳出瀏覽器要求登入,登入一次後就會記住,之後不用再重複。
