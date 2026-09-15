新勢公園 AI 自然偵探｜v3 修正版真 AR

重要修正：
v2 嘗試在手機瀏覽器中即時建立 MindAR target，但 production bundle 並不提供 Compiler，
所以會看到「找不到 MindAR Compiler」。v3 改回 MindAR 官方穩定流程：
先把 3 張目標照片編譯成 targets.mind，再由網站載入辨識。

你只需要做一次：
1. 打開 https://hiukim.github.io/mind-ar-js-doc/tools/compile/
2. 依這個順序上傳 target_sources/ 內三張照片：
   01_demo_color_installation.jpg
   02_water_drop_installation.jpg
   03_river_education_center.jpg
3. 按 Start。
4. 完成後按 Download，得到 targets.mind。
5. 把 targets.mind 上傳到 GitHub Repository 的 assets/ 資料夾。
6. GitHub Pages 更新後，開 ar_test.html 測試。

Target index：
0 = 示範彩色裝置
1 = 水滴裝置
2 = 老街溪河川教育中心

注意：
- 三張一定要照順序一起編譯成同一個 targets.mind。
- 不要改 targets.mind 檔名。
- GitHub 上的路徑必須是 assets/targets.mind。
- 正式活動前仍建議到現場測試辨識距離與角度。
