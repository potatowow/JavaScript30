# Drum Kit

  敲擊不同的鍵盤，播放對應樂器的聲音，並做出鍵盤動畫

### 

### CSS概念

```css
.key {
	border: .4rem solid black;
	border-radius: .5rem;
	margin: 1rem;
	font-size: 1.5rem;
	padding: 1rem .5rem;
	transition: all .07s ease;
	width: 10rem;
	text-align: center;
	color: white;
	background: rgba(0,0,0,0.4);
	text-shadow: 0 0 .5rem black;
}
```

#### 1. flex基本用法  
  - 設定外層display: flex;
  - 給予內層不同flex值，會利用加總的值平均分配寬度(高度)  
  keys {  
    display: flex;  
    flex:1; //會利用內層flex加總的值下去分配  
    align-items : center; //垂直置中  
    justify-content:center; //水平置中  
  }  
  - flex-direction
    有以下幾種值：
      - row（預設）
      - row-reverse（水平反轉）
      - column（垂直）
      - column-reverse（垂直反轉）
      

### javascript 語法
#### <1>keydown監聽
`window.addEventListener('keydown', playSound);`監聽鍵盤
#### <2>建立function `playSound`
1. 取得對應`data-key`的元素
2. 若不是則`return`
3. 對取得的元素進行播放及動畫
4. 設定音檔長度為0，才可以連擊
	
	

比起使用setTimeout讓動畫效果消失，使用Transition end，能夠防止css修改js也必須修改的問題
