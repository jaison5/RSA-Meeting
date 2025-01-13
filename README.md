# RSA-research 
# Academic resources  
[Quantum_polynomial-time_fixed-point_attack_for_RSA](https://github.com/jaison5/RSA-Meeting/blob/main/Quantum_polynomial-time_fixed-point_attack_for_RSA.pdf)  
[Post-Quantum Cryptography](https://github.com/jaison5/RSA-Meeting/blob/main/978-3-319-59879-6.pdf)
# Minutes of meeting  
## 2025/1/1 紀錄  
1.從實務開始學，而不是學整個密碼學，不建議修課  
2.了解RSA的運作方式、實作一遍、了解哪裡被破解，運行目前rsa程式碼或重新撰寫一個  
3.每週報告進度  
4.研究截止：5/15 但做不完也可以投別的  
5.判定論文是否價值： Q1-Q4/ IEEE (量子)  

進度  
1.兩周看完兩篇paper  
2.從了解RSA之運作方式以及各的研究內容
3.模擬運行
 
## **1/13會議記錄**

#### **本週任務**

* 完成 **RSA 破解的數學推導**（第一篇論文）  
* 研究 **橢圓曲線數學**  
* 參考老師新提供的論文，了解可能研究方向、架構

#### **後續計畫**

* **將數學轉換為程式實作**

#### **其他可研究事項**

1. 研究 **橢圓曲線的量子破解模式**  
2. 降低成本（優化計算效率，減少算力需求）  
3. 探索 **可能的商業應用方向**  
4. 研究並模仿 **破解工具的設計方式**  
5. 推導 **RSA 量子數學公式**  
6. 將其他數學推導轉為量子版 (參考論文)

#### **可分工方向**

* **數學推導** vs. **程式開發**  
* **改進 Python 量子模擬**（現有模擬器的改進方案）

#### 可能的額外研究方向

* 比較不同加密方式的安全性與效率

[第一篇論文內容整理](https://hackmd.io/s5iDw7zSSKWp0jns4PjSjA?view#%E9%96%B1%E8%AE%80%E8%AB%96%E6%96%87%E7%B4%80%E9%8C%84)

[筆記共享](https://hackmd.io/s5iDw7zSSKWp0jns4PjSjA?view)

[RSA Demo網站](https://rogerliao0001.github.io/RSA-Demo-site/)

### 老師訊息建議
1. 量子模擬只能跑很小量的測試，是正常的，我提到的 QLSTM 在做第一次測試時的資料集，也超級少，目前這種階段，就是先驗證可行性，不需要大量數據來佐證。因為這時期的困難點，是世界觀的轉換，要怎麼從傳統電腦架構，映射到量子電腦的架構，就是非常有挑戰的 以下是 QLSTM 的相關資料 https://drive.google.com/drive/folders/14_25cxphs_EaSRPXXsNTbMqd8UyQmku3?usp=shar
2. 可以先測試 https://quantumai.google/cirq 在實現 Shor’s Algorithm 的時候，只去破解小型因數分解（像 15、21 之類的數字），是否能執行，就有價值了
3. ttps://colab.research.google.com/github/quantumlib/Cirq/blob/main/docs/experiments/shor.ipynb
4. 透過這樣的詳細對照程式碼與數學推導，你們才能理解，從傳統電腦架構走向量子電腦架構，到底改了哪些
5. 接下來，你理解 RSA 在量子電腦上的運作之後，就可以去參考橢圓曲線的實作 https://gist.github.com/bellbind/1414867/04ccbaa3fe97304d3d9d91c36520a662f2e28a45 以及對應的數學流程教學 https://youtube.com/playlist?list=PLsS_1RYmYQQEun1MTwmvbXurqHIJrFJ0e&si=shofp_XtU3FKXcpd
6. 下次討論，我們先以 RSA 在量子電腦上的模擬運作細節，清楚講一次為主，你們先從這個角度去準備。這樣才能體會量子電腦為什麼可以不需要質因式分解就能破解 RSA，先跑看看 Shor's algorithm
