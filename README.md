# SocialListening (ภาษาไทย)

 Status : `In progress`
 <br><br>
- เนื้อหาในครั้งนี้มาจากการดจดสรุปในความเข้าใจของผมเองหลังจากการเรียน
  - Datarockie : https://data-science-bootcamp1.teachable.com/p/social-listening 
  - Skooldio : https://www.skooldio.com/courses/social-media-data-analytics
  
 <br>
ซึ่งผมมีเจตนาในการแชร์ครั้งนี้เพื่อ <br>
&emsp;1. เพื่อพัฒนาความรู้ตนเอง <br>
&emsp;2. เขียนสรุปในรูปแบบที่ตัวเองเข้าใจ <br>
&emsp;3. เพื่อแชร์ในเนื้อหา/สรุปที่จดให้คนอื่นๆที่ตั้งใจจะหาเนื้อหาในรูปแบบภาษาไทย <br>
<br>
โดยหวังว่าในการแชร์ครั้งนี้จะเป็นประโยชน์กับทุกๆคนที่สนใจหัวข้อ Social Listening นะครับ 

GLHF :smile:

--- 

<h3> Social Listening คืออะไร ? </h3>
&emsp;> คือการวิเคราะห์ข้อมูล โดยที่ข้อมูลดังกล่าวมาจาก Social Media เช่น Facebook, X(twitter), IG, Youtube, Tiktok

<h3>ทำไมต้องทำ Social Listening ?</h3>
&emsp;> เพราะอยากได้ข้อมูล Feedback ของลูกค้า ซึ่งหนึ่งในข้อมูลจำนวนมากที่ค่อนข้างจะรู้ความเห็นจริงๆของลูกค้าก็คือช่องทาง Social Media <br><br>

ป.ล. จากจำนวนประชากรไทย 66 ล้านคน มีคนใช้โซเชียลมากถึง 52 ล้านคนเลยทีเดียว หรือคิดเป็น 75% ของทั้งประเทศที่ใช้โซเชียลมีเดีย   Ref : [Wisesight](https://wisesight.com/news/why-you-should-listen-to-social-media-voice/)
<br>

---

<h3> ขั้นตอนการทำ Social Listening </h3>
&emsp;1. Create a Question (ตั้งโจทย์ว่าเราอยากทำอะไร ต้องหาข้อมูลอะไร  ต้องวิเคราะห์รูปแบบไหน) <br>
&emsp;2. Extract Data (หาข้อมูล) <br>
&emsp;3. Data Preparation + Data Cleansing (จัดเตรียมข้อมูลในมีความเหมาะสม) <br>
&emsp;4. Data Analyst (วิเคราะห์ข้อมูล) <br>
&emsp;5. Presentation (นำเสนอข้อมูล) <br>
<br>

<h4> ในที่นี้ขอแบ่งวิธีการทำ Social Listening เป็นสองแบบหลักๆ </h4>
&emsp;1. ใช้เครื่องมือสำเร็จรูป <br>
&emsp;&emsp;&emsp; ในปัจจุบันมีเครื่องมือสำเร็จรูปมากมายให้ใช้งานจนทำให้เราเหลือแค่ขั้นตอนที่ 1 ที่เราต้องทำเองที่เหลือปล่อยให้เป็นหน้าที่ของผู้ให้บริการก็พอ <br>
&emsp;&emsp;&emsp; เช่น Wisesight, Supermetrics, Zanroo, RealSmart, Brand Watch, Sprout Social, Keyhole, Meltwater, Brand24 <br>
&emsp;&emsp;&emsp; ป.ล. ถ้าทำกับข้อมูลภาษาไทยก็แนะนำให้ใช้เครื่องมือที่รองรับภาษาไทยด้วยนะ <br>

&emsp;&emsp;&emsp;ตัวอย่างการใช้งาน Wisesight  -> [link](https://docs.google.com/spreadsheets/d/1NgOPxZ9Jed-b10pq36DfB5TH6zguxWy77KD44IS5SoY/edit?usp=sharing)
<br><br>
&emsp;2. ทำด้วยตัวเอง <br>
&emsp;&emsp;&emsp; ขึ้นชื่อว่าทำด้วยตัวเอง เราก็ต้องทำด้วยตัวเองทั้งหมดตั้งแต่ 1 - 5 โดยขอยกตัวอย่างวิธีการในแต่ละขั้นตอนตามที่ผมคิดว่าจะใช้งานดังนี้ <br>

&emsp;&emsp;&emsp;&emsp;  2.1 Create a Question <br>
&emsp;&emsp;&emsp;&emsp;&emsp; นั่งอ่านโจทย์แล้วเขียนว่าเราต้องการวิเคราะห์อะไร จะเอาข้อมูลจากไหน นำมาวิเคราะห์อะไร <br>
&emsp;&emsp;&emsp;&emsp;&emsp; เช่น อยากรู้ว่าใน Youtube ช่อง gssspotted คอมเม้นส่วนใหญ่มาแนวโน้มจะ toxic หรือไม่ <br>
&emsp;&emsp;&emsp;&emsp;&emsp; จากโจทย์ทำให้เรารู้ว่า <br>
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; 2.1.1 เอาข้อมูลมาจาก Youtube <br>
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; 2.1.2 ต้องทำ Sentiment Analysis ดังนั้นต้องมี column ที่อธิบายอารมณ์ (positive negative neutral) <br>

&emsp;&emsp;&emsp;&emsp;  2.2 Extract Data (หาข้อมูล)  <br>
&emsp;&emsp;&emsp;&emsp;&emsp; 2.2.1 Web scraping (Python : beautifulsoup, selenium, etc.) <br>
&emsp;&emsp;&emsp;&emsp;&emsp; 2.2.2 API ของผู้ให้บริการ ซึ่งในโจทย์นี้คือ [Youtube DataAPI](https://developers.google.com/youtube/v3) - API มักจำกัดจำนวนการใช้งาน(token)ต่อวันนะ ดูเงื่อนไขดีๆ 

&emsp;&emsp;&emsp;&emsp;  2.3. Data Preparation + Data Cleansing <br>
&emsp;&emsp;&emsp;&emsp;&emsp; 2.3.1 Python library เช่น pandas, regex, os, etc. <br>
&emsp;&emsp;&emsp;&emsp;&emsp; 2.3.2 MSExcel, GGsheet<br>

&emsp;&emsp;&emsp;&emsp;  2.4 Data Analyst (วิเคราะห์ข้อมูล) <br>
&emsp;&emsp;&emsp;&emsp;&emsp; 2.4.1 Python library เช่น pandas, matplotlib, seaborn, plotly, etc. <br>
&emsp;&emsp;&emsp;&emsp;&emsp; 2.4.2 MSExcel, GGsheet เช่น plot graph, pivot data etc.<br>

&emsp;&emsp;&emsp;&emsp;  2.5 Presentation (นำเสนอข้อมูล) <br>
&emsp;&emsp;&emsp;&emsp;&emsp; 2.5.1 Powerpoint, Figma, Canva <br>
&emsp;&emsp;&emsp;&emsp;&emsp; 2.5.2 Dashboard เช่น PowerBI, Looker Studio <br>
