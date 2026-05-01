# 如何打造台版 Edge Impulse TinyML 開發平台
*20260331 許哲豪講師*
## 邊緣智慧VS生成智慧
邊緣式AI特點：
* 運用極少的資源
* 智慧SENSOR
* 超小模型以及低功耗

生成式AI特點：
* 雲端無限資源
* AI生成對話、影像等
* 巨大的資料集、模型

從早期的影像處理（CNN）、語音處理（RNN），進化到現在主流的Transformer架構，進而衍生出大語言模型（LLM）、視覺語言模型（VLM），最終目標是走向具備行動能力的VLA與能團隊協作的Agentic AI。

接著介紹Edge AI講師認為狹義的EDGE AI應該要為只使用電池供電就能完成AI推論的獨立裝置才稱作Edge AI。並且根據不同應用所需的算力也不同

| 智慧感測 | 電腦視覺 | 自然語言 | 生成式對話/繪圖 | 多模態應用 |
| -------- | -------- | -------- | -------- | -------- |
| MOPS     | GOPS     | 1 TOPS     | 10 TOPS     | 100 TOPS     |

並且介紹了EDGE AI該如何開發，分為以下幾個步驟，資料收集->資料標註->模型建置->訓練調參->模型優化->佈署測試，除了以上步驟以外，有些模型訓練還需要前處理以及後處理，講師認為在這些步驟最浪費時間的是資料收集，講師有提到當初他在為百香果園做模型時，耗費了近半年在收集資料，因為不同時間的水果長的樣子不同，同時講師也提到在做模型優化時非常困難，因為要將那麼巨大的模型壓入一些邊緣裝置，並且辨識度不要太低，那個技術非常困難。

講師也介紹了各類的Edge AI開發板，如ARDUINO、新唐、奇景等公司，以及開發Edge AI的軟體，如TensorFlow、Edge Impulse等，也跟我們提到了，arduino以及edge impulse被高通收購。

最後講師跟我們分享了如何利用Edge Impulse製作Edge AI的過程，以及Edge Impulse如何操作。

## 心得報告
最讓我感觸良多的是講師講的「打造台版 Edge Impulse」的產業願景
。身為全球最強大的TinyML免費平台，Edge Impulse已擁有數十萬開發者，被高通正式併購。反觀台灣，雖然是全球主要的 MCU 硬體供應大國，但在MCU AI的軟體開發工具投入上卻相對薄弱。
未來的智慧感測器、工業物聯網乃至穿戴式裝置，都將與Edge AI密不可分。台灣若能結合既有的半導體與硬體製造優勢，自主研發本土的 Edge AI 開發平台，不僅能擺脫對國外軟體生態的過度依賴，更能帶動台灣在軟硬體整合的全面升級。
TinyML正將人工智慧化為設備的「神經末梢」。未來的AI不再只存在於昂貴的電腦中，而是輕巧且無所不在地散佈在我們周遭的每個微小感測器裡。
## 關鍵字
* 邊緣人工智慧 (Edge AI)
* 微型機器學習 (TinyML)
* Edge Impulse
* 模型壓縮與優化 (Model Optimization)
* 微控制器 (Microcontrollers / MCU)
## 參考文獻
* 許哲豪, OmniXRI TinyML 小學堂 (2025) (含簡報檔、直播錄影）
https://omnixri.blogspot.com/2025/06/omnixri-tinyml-2025.html
* 許哲豪, 【課程簡報】20250730_MakerPRO創客交流會─Edge AI 開發平台比一比
https://omnixri.blogspot.com/2025/07/20250730makerproedge-ai.html
* 許哲豪，20251119_MakerPRO_MAI_如何打造台版 Edge Impulse TinyML 開發平台
https://omnixri.blogspot.com/2025/11/20251119makerpromai-edge-impulse-tinyml.html
* MakerPRO, 【2025 MAI Talks】打造台版 Edge Impulse TinyML 開發平台 (YOUTUBE)
https://youtu.be/WSUnU3yagn4
* 許哲豪，邊緣人工智慧實務（EE5354701）─ Ch4. 開源模型推論工具
https://github.com/OmniXRI/NTUST_EdgeAI_2026/tree/main/Ch4_Inference
* 許哲豪，TinyML MCU 等級開源推論引擎
https://omnixri.blogspot.com/2025/06/tinyml-mcu.html
* Edge AI: A Comprehensive Survey of Technologies, Applications, and Challenges
https://ieeexplore.ieee.org/document/10730112
* Opportunities, Applications, and Challenges of Edge-AI Enabled Video Analytics in Smart Cities: A Systematic Review
https://ieeexplore.ieee.org/document/10198424
* Edge Artificial Intelligence in Large-Scale IoT Systems, Applications, and Big Data Infrastructures
https://ieeexplore.ieee.org/document/10470756