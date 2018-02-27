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
