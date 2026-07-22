# **Jodus研究架構規劃大師 🧠**

**Jodus研究架構規劃大師** 是一個專為學術研究者、研究生與指導教授設計的**免費開源、純前端網頁應用程式 (SPA)**。

這是一個將「學術研究方法」與「視覺化心智圖」完美結合的創意沙盒。在撰寫論文緒論或研究計畫書時，常常因為變數關係錯綜複雜而卡關。這個工具讓您可以自由拖曳變數、勾勒出包含自變數、應變數、中介變數與調節變數的複雜因果關係圖，並**自動為您產出學術標準的研究假說與 AI 寫作提示詞**。

👉 [**立即體驗 Jodus研究架構規劃大師**](https://jodusocnncwiy.github.io/research_framework/)

## **✨ 核心特色 (Features)**

* 🎨 **直覺的視覺化畫布 (Intuitive Canvas)**：  
  * 自由新增、拖拉與修改各類研究變數。  
  * 內建標準學術變數標籤：**自變數 (IV)**、**應變數 (DV)**、**中介變數 (MV)**、**調節變數 (MOD)**、**控制變數 (CV)**。  
* 🔗 **高階「中介與調節」連線機制**：  
  * 不再受限於傳統的心智圖點對點連線！您可以將「調節變數」的箭頭直接連向其他兩變數之間的**關係路徑 (因果連線的中央)**，完美呈現學術上「調節效應 / 干擾效應」的視覺化邏輯。  
* 🤖 **即時研究假說與 AI 提示詞自動生成**：  
  * **學術假說自動生成**：根據您的連線與變數類型，系統會自動在下方生成對應的學術假說文字（例如：「假設 H1：【X】對【Y】具有顯著的正向影響」），並且會聰明地**自動過濾掉不需放入主要假說的「控制變數 (CV)」**。  
  * **AI 寫作助理**：根據畫布上的變數，自動生成一段完整的 AI Prompt，您可以一鍵複製並提供給 ChatGPT / Claude 等大型語言模型，快速協助您發想「研究動機」、「學術創新性」及推薦的「理論流派」。  
* 💾 **完整的匯出解決方案 (Export Options)**：  
  * **匯出圖檔 (PNG)**：一鍵下載高解析度 (1200x750) 且無網格背景的架構圖，方便直接插入論文 Word 檔或簡報中。  
  * **匯出計畫大綱 (Markdown)**：自動將畫布上的變數定義、假說清單與 AI 提示詞打包成 .md 檔案下載，無縫接軌您的筆記軟體 (如 Notion, Obsidian) 或直接轉存 Word。  
* 🚀 **流暢的使用者體驗 (UX)**：  
  * 純前端應用，無需後端資料庫，資料全部暫存於瀏覽器的 LocalStorage，即使斷線或不小心重新整理也不會遺失目前的創意！  
  * 支援鍵盤快捷鍵 (Ctrl+Z 復原, Ctrl+Y 重做, Delete/Backspace 刪除)。

## **🛠️ 技術堆疊 (Tech Stack)**

此專案為追求極致的部署便利性，採用單一 HTML 檔案架構 (Single-File Application) 設計，無需 Node.js 環境或繁雜的建置流程即可運行。

* **核心框架**: React 18 (透過 CDN 載入並使用 Babel Standalone 於瀏覽器內轉譯)  
* **樣式設計**: Tailwind CSS (透過 CDN 載入)  
* **圖示庫**: FontAwesome 6  
* **字體**: Google Fonts (Inter & Noto Sans TC)  
* **匯出圖檔引擎**: html-to-image

## **🚀 如何在本機端運行 (Local Development)**

由於整個專案被打包在單一個 index.html 檔案中，部署與測試極度簡單：

1. 將此儲存庫 Clone 到本機：  
   git clone https://github.com/jodusocnncwiy/research\_framework.git

2. 直接用任何現代瀏覽器（Chrome, Edge, Safari, Firefox）開啟 index.html 檔案即可！完全不需要啟動本地伺服器（Localhost）。  
3. *（選用）如果您需要修改程式碼，建議使用 VS Code 搭配 Live Server 擴充功能，以獲得更好的開發體驗。*

## **📚 預設範本教學 (Templates)**

在左側面板提供了三種常見的學術模型供新手直接載入體驗：

1. **經典中介模型 (基礎)**：探討 ![][image1] 的基礎因果機制。  
2. **中介調節模型 (進階)**：展示當 ![][image2] 的過程受到調節變數 (Mod) 干擾時的高階連線畫法。  
3. **超級創意沙盒 (多重因果)**：一個包含雙中介、雙調節以及控制變數的複雜範例，展示本工具處理複雜理論架構的能力，同時示範如何正確生成 AI 提示詞。

## **🤝 貢獻與反饋 (Contributing)**

這是一個自由的開源小工具。如果您對增加新的統計模型建議、更好的介面設計、或是支援不同語言介面有興趣，非常歡迎發起 Issue 討論，或是直接提交 Pull Request！

## **📄 授權條款 (License)**

This project is licensed under the MIT License \- see the [LICENSE](http://docs.google.com/LICENSE) file for details.

[image1]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAHkAAAAaCAYAAACTmvO9AAAEDUlEQVR4Xu1YTUiUQRheycqoiH5s012d3XVJ3IoOS0FRUGFQSQV2KJEigii6REQEXhIiIiIIDIJQrC6VVOJBSIiKvFSXThZUEIIk2CGIFEpye57d+Xanadt2v59dk3ng5ZuZ952Z92fmfWfX5zMwMDAwMDCYdqitrY0JIT6AEgpN1NTUbCYf7Q6N9zESiazU1ykVQqFQC3T6pujXj7EKXc4CeMcV2R+w/2Yuea8BHU5TD0WnBPR5HggElloywWAwivERRSYdn4KAiRtA30HvQVXWeDQanYt+L5xxzu/3z1fnTBcwSKB70PMzaLC+vn6hLkPQWbBjADKToAs6v4Qogz7XZACz6gX7dkD3l7yUOi9vwAHzsMAjbDLFBeUwNz9DYluVn06A7gHoeBv0ADSsHlIL8Xh8NsbbYONF6cydukwpAb02idThe4FMuUjlhcNhgZj08auO2wIWOiAdcEc6hQG+zLYu6xZgXBy0XR8vBHQQdL+E71noO841dRkGFdQMXje+o/hGdBmncGILA8sAM9C0xxqHXSsw1osAr1flbQML+bHgW9AX0HlQh5cBJlBbVmOfKz4HmUIGt1lSggFV+XV1dcvhrHZ544dAj70oPU5toY5S/2TKloHvB+3TZR2BG3AjFn89bXiEcjom2+3LE+WYex1rNODbiO8UqFXhl2H8JGgV9wBv3HKiB3Bki8i8i4bkgexAHA77bB6avwIL75KO+qM2eAXWGqCTqUnn/QtWPeZjC+usRfsrqM3iM83B6UfZxvrHRJab7iac2FJZWbkAc59J/z8VXryFsGgD6AkUfMeNQpkHWN5gepdpv6pAahKpmrTNV4BhrF+sx2zLdYbRv8U+ncYUKA8rb3S3KKAeF9sWQpaeBHV1vVTyBMIhffyZEVIeYGCV67K5gDkbQTdsUBfoE+h1IenOqsds8zajPShkzQXvEA8BedXV1ctEgfVYFNkWQqTK5RTmNeo8R5AFvoepjX15epMPMD4mdHm3wROLg3UV+x1Bd5bOz4F0Pbb6aN8HDWG9LSKVtpM3CXasQ3+CTsxMdx8ObGE5qRCph9ZIIBAI6nzbkAF+CGpSx5nmROoB1q6OewHs0yps1B9Zj3sQ6MXWGPqdoDGmbNVRoSLUY8KuLQTLCOaOMtAMuM63BSwWZooGndJ5THPgT4L3Sv2LzW0wa7D+2HjklUG3Fs5l2xqU6Zvvif0Z0fQNz7se24EDW5JAttkjD2L64WgbUOSg+P3/0p9wyl6Lj/4Jjql8zBnAzVmiruMGWHuyHbJcyKI/X9RbJW832j1Mm7Iu39Vk+T93VywWm6Ov6xR2bCFCqf/TxxQdSW/g7zW67H8JpiXXUlOJMZNsMTAwMDAwMDAwMDAwMDCYSfgFOzNla70M4B0AAAAASUVORK5CYII=>

[image2]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEkAAAAaCAYAAAD7aXGFAAADFUlEQVR4Xu2XTUiUQRjHV7IvKqIP23RXZ3ddkragw1JQFFQYVBKBlxKpQxBFl+gQgZeEkIgIAg9BKFaXSvqgQ5AQHfIiXTpFUEF4KahDECmkpP3+7bw2DaL7Ze7h/cOfmXmeZ56ZeeaZ592NREKECBGiQtHQ0JAxxnyAkw5H6+vrd0lPv9vTfUylUht8P/OFRCLRxp5+OPt7imyJbxcA3WnHdozz35rJ/h8wYTv8Cd/D2kCeTqcXM36Ms4vRaHSZO6dSoEPC++zzKxxsampa4dsI8Xg8zTkGsBmHXb5+VuBgKQ6eMXmCBfdbcRXj86L6rn0lgb3H2OMd+BAOu5ccIJvNLkTewRkvm1wWHfBt8gLBOWod3LVOFaCr6vu25QKbzsJ9vrwQMH8ne79Ce4H9jsinb6OgwFZ0fbSfaVO+TV5IJpNRHLyF3+Al2D2XARKofZtZ51qkhEy1wWm1nFRAXH1jY+M6gthpM+4NfF5S6cBBlxbC6UsK9EpfPweoVpCmu/08Uc3cG/jYSNtMOwHbHX0V8rNwk9ZAN6IzOvrCgYODdqGh/xQkZTDLmR4uZr2vmw1BPVKxxs8W+t9hR6BHto3gnFQf/6eUAKbYeiToNuALnL1ToJwCnjf0PO2zrS2QLXAI7o0U8PSCeqS+9TPM+LbGNTU1y/XM7GUro/pMifXI4PCJPpNuAUdV7dvOBObsgDeLYC/8BF8X8vSCeqS+son+oLE1B91xBVG6urq6taaUeqRIM7lfqamxW8BVWH37ckPZx8VcZ70TDBf4+hkwVY+CMf0HCgb+dpvcs/uTlZxjK+NRU0w9sgF6BFtcudLU5Ap4pyufC7BOuynit5itR/0EalUgY9wDv+jJxWKxeCAvuh4xIaknBs/5OqUp+nF0r1hsja8vF5S1qhVFfCSq2Fub5qofCO3zUz098td0KsPyr0cYHmPCmI2s+AunhwM94zOSuXrmDHBzq10/5QB+m6e7pJkwzf71RdtjdYfo9+sJ27p0z7PV/7zeTCazyPdbsUjk/nfl9wczRIgQIUKECBEixLzjNyjo9142P/8PAAAAAElFTkSuQmCC>