## Chapter 21: Functions
It is my coding practice with the TUTORIAL of Dave Gray. 

## Source
### Dave Gray 的 CSS 資源
https://github.com/gitdagray/css_course

### Dave Gray 的 CSS 課程
https://youtube.com/playlist?list=PL0Zuz27SZ-6Mx9fd9elt80G1bPcySmWit

### Dave Gray 的 YouTube 頻道
https://www.youtube.com/@DaveGrayTeachesCode

## Quick Concept outline
###  1. Intro
        教學影片固定的開頭

###  2. Welcome
        歡迎觀眾，說明工具與資料位置

###  3. Starter Code
        初始設定說明

###  4. CSS functions we already use
        說明先前使用過的 CSS 函數

###  5. min function
        修改 :root 的 -FS 為 min(2.25rem, 3vh)，min 通常提供較大的絕對值

###  6. Quick page adjustments
        (1)修改 main，並設定 display 為 flex，flex-flow 為 column nowrap，justify-content 為 flex-start
        (2)修改 padding 為 var(--PADDING)，刪除 nav 的 padding，修改 :root 的 --PADDING 為 0.5em，

###  7. Unit choices
        絕對單位: rem
        相對單位: %, vh
        2.25 rem = 36px
        100% = 16px

###  8. max function
        修改 :root 的 -FS 為 max(1.75rem, 3vh)，max 通常提供較小的絕對值

###  9. clamp function
        修改 :root 的 -FS 為 clamp(1.75rem, 3vh, 2.25rem)

### 10. Add an aside with calc and clamp
        (1)新增 :root 的 -FS-SM 為 clamp(1.25rem, 2vh, 1.5rem)。
        (2)新增 main section 的 flex-grow 為 1，padding 為 --var(--PADDING)
        (3)新增 main aside 的 背景色為 hsla(0, 0%, 20%, 0.8) 和文字色為 var(--LIGHT-COLOR)、字體大小為 var(--FS-SM)、字型為 italic斜體，padding 為 var(--PADDING)
        (4)設定 media query 最小螢幕寬度為 576px，main 為 flex-flow 為 row nowrap，justify-content為space-between。
        main section 的 寬度為 70% - 5px。
        main aside 的 寬度為 30% - 5px。
        在 html　新增 aside 內容。

### 11. Small adjustment
        設定 .content 的 margin-top 為 20px

### 12. filter functions - brightness, hue-rotate
        (1)設定超連結顏色為 firebrick火磚色，
        設定滑鼠游標懸停和 tab 選取，透明度為 0.6
        (2)修改滑鼠游標懸停和 tab 選取，filter 為 brightness(150%)
        (3)修改 filter 為 hue-rotate(180deg)

### 13. Create a tooltip with attr function
        (1)設定 .tooltip 的 border-bottom 為 1px dashed orange
        (2)設定 .tooltip 的 position 為 relative
        (3)設定 .tooltip:hover::before 的 content 為 attr(data-tooltip)，
        position 為 absolute，
        top 為 -20px
        (4)設定 white-space 為 nowrap，
        背景為暗色，
        padding 為 var(--PADDING)，
        border-radius 為 15px

### 14. Grid functions - repeat, minmax
        (1)修改 html 和 CSS 的 main 樣式，flex-grow 為 1，display 為 grid，grid-template-columns 為 repeat(4, minmax(100px, 300px))，gap 為 min(2vw, 20px)
        (2)移除 .square 的 寬度和高度
        (3)設定 padding 為 var(--PADDING)，
