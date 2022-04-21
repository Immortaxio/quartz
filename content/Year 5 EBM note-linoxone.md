#EBM #Statistics 
# Intro
- EBM = best evidence with ==clinical expertise== and ==patient values==
- คุณภาพ = clinical ==relevant==+ ==valid==
- Flow การทำงาน หลักๆ คือ
	1. ตั้งคำถาม (PICO)
	2. หาหลักฐาน (evidence)
	3. วิเคราะห์ วิพากษ์ (appraise)
	4. เอามาใช้จริง ได้ผลไหม (apply & evaluate)

## Data
![400](https://i.imgur.com/VQSYvKL.jpg)
## Errors
1. Systematic = bias เพี้ยนอย่างมี direction แก้ด้วย study design คุณภาพ
2. Random = chance เพี้ยนมั่ว (unpredictable) แก้ด้วย statistic ที่ดี

![400](https://i.imgur.com/lzVahFt.png)
- $\alpha$ กำหนดตั้งแต่ต้น ใช้คำนวณ [[sample size]] ร่วมกับ primary outcome
- power = โอกาสที่จะ detect ความต่างได้

## Randomization
	3 Keys-> ชนิดไหน, ปกปิดยังไง, balance ไหม
- เพื่อ ลด bias (selection)
- stratified -> ลด coufouding ได้ดี
- block randomization เป็นแค่ restricted $\neq$ true randomization 
## Study designs
## Biases
|Types|Solutions|
|-|-|
|selection|balanced randomization|

Details
- selection(allocation)
- 

# Biostats
- p-value < 0.05 ลด alpha error | power > 90% ลด beta error
- PPV~1/NPV~prevalence
- NNT = 1/ARR
- Post-test odd = pretest odd x LR
    - odd = prob/1-prob
    - prob = odd/1+odd
    - LR = True positive/False positive
    - LR+ >10 good
    - LR- <1/10 good
- หา accuracy test จากกราฟ ใช้ AUC of ROC curve เข้าใกล้ 1 ดี
- surrogate outcome เหมาะในการเป็นตัวแทนโรคร้ายแรง
- Pragmatic trial เน้น external validity + clinical relevant (effectiveness)
- Explanatory trial เน้นตอบคำถาม work ไหม efficacy เป็นยังไง
- Phases
    - 1 = safety
    - 2 = dose range
    - 3 = clinical trial
    - 4 = market

- split body = 2 intervention ในคนเดียว เช่น รูจมูก 2 ข้าง
- Blinding
    - ไม่ได้ทำได้เสมอ ไม่ได้ลด measurement bias เสมอไป
    - The must in RCT ?
    - statistician should ?
- power calculation หรือการเพิ่ม [[sample size]] มีเพื่อลด random error ไม่ได้จัดการ bias
- Dichotomus data = binary data = yes/no high/low male/female dead/alive



![400](https://www.dropbox.com/s/cqy3jr13xn4nw0g/IMG_0178.png?raw=1)


![400](https://www.dropbox.com/s/r0s5hroqvvp988x/IMG_0179.webp?raw=1)
![400](https://www.dropbox.com/s/36thozxg9ut6pb5/IMG_0180.jpeg?raw=1)


# Bio-informations
	Keys -> Scopus 1960 > Pubmed 1945 > Medline
	- Pubmed search[options] L-R
	- Scopus options["search"] OR-AND-NOT
- clinical key ยุ่งยากสุด
- citations ดูใน scopus ได้ทั้งไป-กลับ ส่วน pubmed ดูไม่ได้
- google scholar หาจาก full  text เลยไม่เหมือนเจ้าอื่นใช้แค่ abstract +ชื่อต่างๆ

## Pubmed
	Keys -> ดู search detail ทุกครั้ง, MeshTerm, ATM
- หา author ใส่ [AU] ด้านหลัง
- อยากเห็น Find it @chula ต้องเข้าผ่าน link หสม
- advance search
- ต้องเข้าใจการทำงาน pubmed !!!

### Automatic term mapping(ATM)
ทำให้ค้นหาง่าย easy keyword เพราะจะแมพเข้า meshterm อัตโนมัติเลย
### Meshterm (Medical subject heading)
ช่วยให้หาได้กว้างขึ้น โรค/ภาวะเดียวกันพิมพ์คำ variation ไหนก็เจอ สะดวกดีนะ
- แต่ เหมือนเป็น hashtag ต้องรอคนมา add ใส่ paper ใหม่ๆ 
- แต่ โรคใหม่ๆ ต้องรอคนสร้างก่อน
- แต่ paper โบราณ ตีพิมพ์ก่อนมี meshterm ก็เข้าไม่ถึง
- แต่ บางทีมีแถมคำที่ไม่ต้องการ

 ## ห้องสมุด 
- ยืม paper ข้ามหสม 5 บาท  แต่ถ้าจากเครือ WHO ฟรี
- หาแบบ Title จะต้อง==ขึ้นต้น==ด้วยคำนั้นเลย ไม่เหมือน keyword ==อยู่ตรงไหนก็ได้==
- ไปดูพวก volume วารสารมีให้ยืมไหม


|Scholar|Scopus  |Pubmed  |
|---|---|---|
|med and non-med|med|med|
|  |  |ชินกับคำค้น Meshterm ก็มี, tagging ทำให้หาง่ายกว่าในด้าน filter, ภาษามากกว่า update กว่า pubmed|
|  |  |  |


# Analysis
- post-hoc ไม่น่าเชื่อถือ และถ้าข้อมูลหายจะทำไม่ได้
- interim
    - good for ? :: severe disease (stop before danger)
- Network analysis = หา A-B ไม่ได้ เอา A-C subtract B-C แทน เพิ่มจำนวน paper
- NI trial ดูจากการคร่อม margin ฝั่ง?::control  
- Regression analysis

|  Outcome|  Test|
|---|---|
|  categorical|  linear|
|  continuous|  logistic|
|  time to event|  cox proportional hazard|
|  incidence rate|  poisson|

# Diagnostic
- หา sense, spec, PPV, NPV, accuracy, LR+, LR-
- ถ้าเปรียบเทียบ Test A-B ใช้ ROC curve -> หาพื้นที่ AUC ใกล้ 1 สุด (มากสุด) = best
- $LR+ = \frac{sense}{1-spec}$
# Prognosis
- อยากรู้ว่า นานเท่าไหร่ถึงตาย เลยต้องทำ survival analysis แทนการทำ chi square
- ใช้ time to event -> จำนวนเวลาที่มี hazard แต่ยังรอด คือ survival time 
- loss f/u เอาที่เคยเก็บมาใช้ได้
- ดูโอกาสรอดชีพ(survival) ธรรมดา ใช้ Kaplan-Meier curve แสดงได้
- ถ้าจะ compare ระหว่าง ยา A-B -> ใช้ log rank หลักการคล้าย  $\chi^2$  test
- ถ้าจะสร้าง model เลย predict โอกาสรอดได้จาก risk factors ->  Cox proportional hazard regression
	-  HR > 1 แปลว่า เพิ่ม risk
# RCT
	Keys -> intervention ทำ NI ก่อนไป superior (Heirachy testing)
- NI ควรมีทั้ง ==ITT + PP== analysis ที่ agree กัน เอา margin มาจาก previous study
- NI ใช้ [[sample size]] > PP  `verify?
- Composite endpoint
	- เอาหลาย outcome มัดรวมกัน เพราะแต่ละอันอาจมี sample น้อยเกินไป ทำให้ power ไม่พอ detect ความต่าง
	- ถ้าผล sig ต้องมาแยกว่าอันไหนตัวเด่น (event driven)

# Systematic review and metaanalysis
- forest plot ดู result ของ studies ที่รวมเข้ามา
- funnel plot ดู publication bias
# Economic
- Intangible cost = pain and anxiety
- Capital cost = resource with half-life > 1 year 
- คำนวณ utility index `???`
- ICER = ความต่าง cost/ความต่าง effective ใช้เทียบ new treatment/technology
        - ถ้าได้ผลเท่ากัน คำนวณไม่ได้ 555
![400](https://www.dropbox.com/s/s4wuhvac095tlpb/IMG_0168.png?raw=1)

# Ethics
- ตีพิมพ์ซ้ำได้ ต้องขอวารสารแรกก่อน ไม่งั้นผิด copyright
- [[Plagiarism]] ไม่ผิดกฏหมาย
- [[Copyright]] ลิขสิทธิ์ คุ้มครอง==ทันที==ที่สร้าง ==expression== $\neq$ idea 
- [[Patent]] สิทธิบัตร เครื่องหมายการค้า

# Spot dx
![400](https://www.dropbox.com/s/5uy9hfm42deqcr5/IMG_0174.png?raw=1)
![](https://www.dropbox.com/s/tyk5pnguuoie13u/IMG_0175.png?raw=1)
![400](https://www.dropbox.com/s/nq26innrv2h45kc/IMG_0177.png?raw=1)
![400](https://www.dropbox.com/s/z07j7rtb5fs3jml/IMG_0169.png?raw=1)
![400](https://www.dropbox.com/s/rwt5wp59x7a1i8o/IMG_0172.png?raw=1)


# MEQ 
1. สรุป paper นี้ น่าเชื่อถือไหม ?
	- case-control
	- cohort
	- prognosis
		- new Dx เกณฑ์ชัดเจน ระยะเดียวกัน 
		- f/u นานพอ ไม่ loss >20%
		- objective outcome เถียงไม่ได้ 
		- ทำใน population-setting ไม่ใช่โรงพยาบาล
2. สรุป paper นี้ เอาไป apply ได้ไหม ?
	- patient characteristic and exposure เหมือนไหม
	- f/u time นานพอไหม
