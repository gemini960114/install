幫我用 MultiQC 把一堆 QC 報告整合成一份好看的 HTML 報告。整個專案放在一個叫 `multiqc-report` 的資料夾裡。

情境是跑完定序分析後,會有一堆工具各自產生的報告檔案散在不同資料夾(像 FastQC、samtools 之類的),想要一個指令就能把這些全部掃過去,彙整成一份總覽報告,方便一次看完所有樣本的品質狀況,不用一個一個檔案打開看。

用 uv 裝 MultiQC 就好,跑完直接開瀏覽器看那份 HTML 報告。

手邊沒有現成的報告資料的話,可以去 https://github.com/MultiQC/test-data 這個 repo 抓,裡面有各種工具(FastQC、samtools 等等)的範例輸出,clone 下來挑一個資料夾直接跑就能看到效果,不用自己真的跑一輪定序分析。
