# Korean_Movie_review_emotion_prediction_using_deep_learning

***Korean movie review emotion prediction using deep learning***

This simple project predicts korean movie review based on naver movie review web.  
See requirements.txt before testing and check detail through source code๐  

---

## 1_Crawling  
![12](https://user-images.githubusercontent.com/120359150/213603825-a6841028-e624-43fc-9e20-0e008c3f6cfe.PNG)  
https://movie.naver.com/movie/point/af/list.naver  
Crawling upper web using 'Data_crawling.ipynb'  
โThis web pages is maybe limited 500 pagesโ  

## 2_Labeling
This project case, using 3 label(0: Negative / 1: Positive / 2: Normal)  
But I recommend just using 2 label(0: Negatice / 1: Positive).  Because most reviews are 'positive', There is a data imbalance.  

## 3_Preprocessing & train  
See detail through this source code.  
In this project case, just used only Bi-LSTM. If you have a good idea, try applying!

## 4_Test  

**Input for testing**
| Label | Input sample |
| :--- | :--- |
| Positive | ์ด ์ํ ๋๋ฌด ์ฌ๋ฐ๋ค~~!! |
| Negative | ์ด๊ฑฐ ๋ณด์ง ๋ง์ธ์ ์ง์ง ์ฌ๋ฏธ ์์ด์ |
| Negative | ํ๊ฐ ์๊น์ |
| Normal | ์ด๋ฐ๋ถ ์ ์ธํ๊ณ  ์ ๋นํ ๋ณผ๋งํด์ |
| Positive | ๋๋ฌด ๋ชฐ์ํด์ ๋ดค๋ค์ ์๊ฐ๊ฐ๋ ์ค ๋ชฐ๋์ |

**Result**  
**๐please modify: batch_size = 4**  
![1](https://user-images.githubusercontent.com/120359150/215250054-61fbe765-6635-4a40-8407-992bdc6b2baf.PNG)  
