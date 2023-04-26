# Markdown圖表 社課實作示範

> Created by 王修佑 (GitHub [@whyhugo](https://github.com/whyhugo))<br>
> [GitHub README.md](https://github.com/whyhugo/Handouts/blob/main/Markdown%E5%9C%96%E8%A1%A8%E5%AF%A6%E4%BD%9C.md)<br>
> [HackMD](https://hackmd.io/@whyhugo/rkMEGXnH9)

### 2022/04/29 社課X 
## Gantt Chart
- 可用於顯示專案、進度以及其他與時間相關的系統進展的內在關係隨著時間進展情況的圖表，現今被相當廣泛的運用。

```mermaid
gantt
%% 宣告圖表樣式gantt
    title 以機器學習研究計畫為例
		%% 圖表標題
    dateFormat  MM-DD
		%% 日期格式
		axisFormat  %m-%d
		%% 縱軸的日期格式
		
		section 前期工作
		%% 宣告一個區塊
		    Conceive project : crit, done, plan, 04-11, 28d
			%%語法：
			%%甘特圖上的任務名稱 : [crit], [active|done], 任務名稱, [日期|after 任務名稱], 長度

		
        section 預處理
            Rlated Work  :active,bb, 05-02, 42d
            Collect & extend datasets  : crit ,b2, 05-09, 56d
    
		section 主要工作
            Data preprocessing: active, dp, 06-13  , 35d
            Model tuning: implement, after dp, 63d

		section 研究收案
			Analysis & Evaluation: copyright, 07-25, 70d
            Discussion & conlcusion: dc, 08-08, 72d
			
        section 發表工作
            Writing & Modifying report: wm, 09-05, 49d
            Presentation: milestone, after wm, 7d
```
👉[開啟HackMD雙欄模式檢視原始語法](https://hackmd.io/T-UpzCz-QV-AMSDCmXIVUw?both)  
- 原始碼Open Code
````
```mermaid
gantt
%% 宣告圖表樣式gantt
    title 以機器學習研究計畫為例
		%% 圖表標題
    dateFormat  MM-DD
		%% 日期格式
		axisFormat  %m-%d
		%% 縱軸的日期格式
		
		section 前期工作
		%% 宣告一個區塊
		    Conceive project : crit, done, plan, 04-11, 28d
			%%語法：
			%%甘特圖上的任務名稱 : [crit], [active|done], 任務名稱, [日期|after 任務名稱], 長度

		
        section 預處理
            Rlated Work  :active,bb, 05-02, 42d
            Collect & extend datasets  : crit ,b2, 05-09, 56d
    
		section 主要工作
            Data preprocessing: active, dp, 06-13  , 35d
            Model tuning: implement, after dp, 63d

		section 研究收案
			Analysis & Evaluation: copyright, 07-25, 70d
            Discussion & conlcusion: dc, 08-08, 72d
			
        section 發表工作
            Writing & Modifying report: wm, 09-05, 49d
            Presentation: milestone, after wm, 7d
```
````
### 👍好站推薦
- [如何繪製甘特圖](https://hackmd.io/@hackmd-marketing/draw-gantt?utm_source=twitter&utm_medium=post-link)
- [Mermaid.js document](https://mermaid-js.github.io/mermaid/#/gantt)

## Pie Chart
👉[開啟HackMD雙欄模式檢視原始語法](https://hackmd.io/T-UpzCz-QV-AMSDCmXIVUw?both)
```mermaid
pie

title Animals

"Dogs" : 52.8
"Cats" : 24.8
"Rats" : 8.6
"Dragon" :  4.0
"Lion": 8.9
```
- 原始碼Open Code
````
```mermaid
pie

title Animals

"Dogs" : 52.8
"Cats" : 24.8
"Rats" : 8.6
"Dragon" :  4.0
"Lion": 8.9
```
````
### 👍好站推薦
- [畫圖真的好簡單](https://hackmd.io/c/tutorials-tw/https%3A%2F%2Fhackmd.io%2F%40docs%2Fmermaid_pie?fbclid=IwAR0dQVb-373PL-57PhsdOWoOFYgh2j1JrA78hwTzD6NP92q6XY90X9jD5g0)

## Flow Chart
👉[開啟HackMD雙欄模式檢視原始語法](https://hackmd.io/T-UpzCz-QV-AMSDCmXIVUw?both)
```mermaid
flowchart TD
A([Start]) --> B{"TASK😎"}
B -->|Yes| C["OK"]
C --> D[Rethink]
D --> B
B ---->|No| E["End"]
```
- 原始碼Open Code
````
```mermaid
flowchart TD
A([Start]) --> B{"TASK😎"}
B -->|Yes| C["OK"]
C --> D[Rethink]
D --> B
B ---->|No| E["End"]
```
````
## Sequence Diagram
👉[開啟HackMD雙欄模式檢視原始語法](https://hackmd.io/T-UpzCz-QV-AMSDCmXIVUw?both)
```mermaid
sequenceDiagram
  Alice->>John: Hello John, how are you?
  loop Healthcheck
      John->>John: Fight against hypochondria
  end
  Note right of John: Rational thoughts!
  John-->>Alice: Great!
  John->>Bob: How about you?
  Bob-->>John: Jolly good!
```
- 原始碼Open Code
````
```mermaid
sequenceDiagram
  Alice->>John: Hello John, how are you?
  loop Healthcheck
      John->>John: Fight against hypochondria
  end
  Note right of John: Rational thoughts!
  John-->>Alice: Great!
  John->>Bob: How about you?
  Bob-->>John: Jolly good!
```
````
## State Diagram
👉[開啟HackMD雙欄模式檢視原始語法](https://hackmd.io/T-UpzCz-QV-AMSDCmXIVUw?both)
```mermaid
stateDiagram
  [*] --> Still
  Still --> [*]
  Still --> Moving
  Moving --> Still
  Moving --> Crash
  Crash --> [*]
```
- 原始碼Open Code
````
```mermaid
stateDiagram
  [*] --> Still
  Still --> [*]
  Still --> Moving
  Moving --> Still
  Moving --> Crash
  Crash --> [*]
```
````
## Class Diagram
👉[開啟HackMD雙欄模式檢視原始語法](https://hackmd.io/T-UpzCz-QV-AMSDCmXIVUw?both)
```mermaid
classDiagram
  Class01 <|-- AveryLongClass : Cool
  <<interface>> Class01
  Class09 --> C2 : Where am i?
  Class09 --* C3
  Class09 --|> Class07
  Class07 : equals()
  Class07 : Object[] elementData
  Class01 : size()
  Class01 : int chimp
  Class01 : int gorilla
  class Class10 {
    <<service>>
    int id
    size()
  }
```
- 原始碼Open Code
````
```mermaid
classDiagram
  Class01 <|-- AveryLongClass : Cool
  <<interface>> Class01
  Class09 --> C2 : Where am i?
  Class09 --* C3
  Class09 --|> Class07
  Class07 : equals()
  Class07 : Object[] elementData
  Class01 : size()
  Class01 : int chimp
  Class01 : int gorilla
  class Class10 {
    <<service>>
    int id
    size()
  }
```
````


###### tags: `zfcsc`

