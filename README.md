# autogirl_prompt
auto build girl prompt for stable diffusion
這是一個自動產生美少女的prompt，他會以亂數的方式，產生不同髮型，髮色，服裝與背景顏色的少女圖像。<br/>
https://github.com/vinshagit/autogirl_prompt/<br/>
首先要使用它必須先安裝dynamic-prompts<br/>
https://github.com/adieyal/sd-dynamic-prompts.git<br/>

我們主要使用dynamic-prompts中的wildcards功能<br/>
<br/>
* 1.0版<br/>
<br/>
請下載1.0目錄裡的所有檔案。<br/>
然後複製hair_color.txt與backgrounds_colors.txt 到（你的stable-diffusion-webui）\extensions\sd-dynamic-prompts\wildcards
prompt.txt 的內容貼到stable-diffusion 正反prompt還有各項參數。<br/>
我有使用一些負面 ti：EasyNegative,bad-image-v2-39000, bad_prompt_version2, EasyNegative,NG_DeepNegative_V1_4T,bad-artist-anime:0.7),k,bad-hands-5<br/>
如果你沒有安裝，可以去下載，或是忽視它換成自己的負面題詞<br/>
你就可以自由地算圖，每次產生的圖都不同的髮型，髮色，服裝與背景顏色<br/>
這版的prompt我建議使用主模型 breakdomainrealistic或ghostmix<br/>
當然你可以試試換成你喜歡的模型<br/>

<br/>
* 2.0版<br/>
請下載1.0目錄裡的所有檔案。<br/>
然後複製hair_color.txt,shoes.txt,job.txt與backgrounds_colors.txt 到（你的stable-diffusion-webui）\extensions\sd-dynamic-prompts\wildcards<br/>
請到webui的wildcards Manager tab頁面，使用Refresh Wildcards按鍵，刷新增加的wildcards內容<br/>
<br/>
2.0除了調整畫質的tag，職業,衣物與鞋類的內容放到wildcards的目錄中，而背景也換成各種場所，而不是單色背景。<br/>
{__clothes__,__shoes__|__job__}這樣的語法讓職業或衣物鞋子只會選擇其中一種<br/>
你也可增加一些風格性的lora，也許會到更好的結果。<br/>

