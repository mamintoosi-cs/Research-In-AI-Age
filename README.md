---
marp: true
title: Research in the AI Age
theme: gaia
class:
  - invert
paginate: true
size: 16:9
author: Mahmood Amintoosi
transition: fade
direction: rtl
backgroundColor: '#88735dff'  
style: |
  section {
    font-family: 'Vazirmatn', 'B Nazanin', 'Tahoma', sans-serif;
    direction: rtl;
    text-align: right;
  }
  h1, h2, h3 {
    text-align: center;
  }
  h6 {
    text-align: left;
    direction: ltr;
  }
  code {
    direction: ltr;
    text-align: left;
  }
    /* تنظیم مستقیم برای عناصر عنوان */
  section:first-of-type h1 {
    margin-top: 120px;
  }
  section:first-of-type h2 {
    margin-top: 30px;
  }
  table {
  width: 95%;
  margin: 0rem auto;
  border-spacing: 30px;
  border: none;
  }
  th, td {
    text-align: center;
    font-size: 0.95em;
  }
---

<!-- ![bg cover opacity:.7](img/title-page..jpg) -->

![bg right](img/20th-century-enhanced.jpg)

![width:480](img/besm.png)

<!-- بسم الله الرحمان الرحیم -->

### پژوهش در عصر هوش مصنوعی

### فرصت‌ها و چالش‌ها

**محمود امین‌طوسی**
دانشکده علوم ریاضی - دانشگاه فردوسی مشهد

[mamintoosi.github.io](https://mamintoosi.github.io/)

آخرین به‌روزرسانی: آبان ۱۴۰۵ (اکتبر ۲۰۲۶)

<!-- _footer: گروه علوم کامپیوتر   -->
<!-- _paginate: false -->

---

![bg right](img/mAmintoosi-50.jpg)

## تمام تصاویر و ویدئوهای این ارائه که در آن تصویر اینجانب آمده است با هوش مصنوعی مولد و فقط با دادن این عکس و دستور متنی تولید شده‌اند

---

## ساختار کارگاه: دو نشست ۹۰ دقیقه‌ای

**نشست ۱ — مبانی و آموزش**
- هوش مصنوعی مولد، مدل‌ها و عامل‌ها (Agent)
- مهندسی پرامپت
- AI در آموزش: تکلیف، بازخورد، ارزیابی

**نشست ۲ — پژوهش**
- ابزارهای پژوهش و مرور ادبیات
- مطالعه موردی: از ایده تا پیش‌نویس مقاله
- اخلاق، سیاست نشر و راستی‌آزمایی

**پیوست:** فرصت‌ها در علوم کامپیوتر

---


![bg right](img/poster.jpg)
![bg right](img/old-new-era.jpg)

## سرفصل‌های ارائه

1. نشست ۱: هوش مصنوعی مولد، عامل‌ها (Agent)، پرامپت و آموزش
2. نشست ۲: ابزارهای پژوهش، مرور ادبیات و مطالعه موردی
3. اخلاق، سیاست نشر و راستی‌آزمایی
4. پیوست: فرصت‌ها در علوم کامپیوتر

---

# نشست ۱

## مبانی و آموزش

---


![bg opacity:0.3](img/Gen-AI.webp)

## بخش اول

## هوش مصنوعی مولد: انقلاب در پژوهش

---

![bg opacity:1](img//Trial-01-01.jpg)

| گذشته:            | امروز:                  |
| :---------------- | :---------------------- |
| جستجو در Google   | دستیارهای هوشمند پژوهشی |
| مطالعه صدها مقاله | خلاصه‌سازی خودکار       |
| نگارش دستی        | کمک در نگارش و ویرایش   |
| کدنویسی از صفر    | تولید کد با AI          |

<style scoped>
table {
  width: 45%;
  margin: 0rem auto;
  border-collapse: separate;
  border-spacing: 30px;
  border: none;
}
th {
  text-align: center !important;
  font-size: 1.5em;
  border-bottom: 2px solid #333;
  padding-bottom: 1px;
}
td {
  text-align: right;
  vertical-align: top;
  border: none !important;
  padding: 1px;
}
td:first-child {
  border-left: 3px solid #888;
}
td:last-child {
  border-right: 3px solid #888;
}
</style>

---

<!-- html -->
<div style="
  display: flex;
  justify-content: center;
  align-items: center;
  height: 80vh; /* یا 85vh */
  margin: 0 auto;
">
  <div style="
    width: 80%; /* یا 80% */
    text-align: center;
  ">
    <video 
      controls 
      style="
        width: 100%;
        height: 70vh; 
        border-radius: 12px;
        box-shadow: 0 6px 20px rgba(0,0,0,0.25);
        background: #000; 
        object-fit: contain; 
      ">
      <source src="img/Research-Accelerator.mp4" type="video/mp4">
      مرورگر شما از تگ ویدئو پشتیبانی نمی‌کند.
    </video>
  </div>
</div>

---

![bg opacity:0.3](img/AI-gemini-generated.jpg)

### هوش مصنوعی مولد چیست؟

- **تعریف:** مدل‌هایی که براساس الگوهای یادگرفته‌شده از داده‌ها، محتوای جدید «تولید» می‌کنند

- مانند یک نویسنده، نقاش، یا برنامه‌نویس

| نام مدل        | شرکت/توسعه‌دهنده | وب‌سایت                                                  |
| :------------- | :--------------- | :------------------------------------------------------- |
| **ChatGPT**    | OpenAI           | [chatgpt.com](https://chatgpt.com)                       |
| **Claude**     | Anthropic        | [anthropic.com/claude](https://www.anthropic.com/claude) |
| **Gemini**     | Google           | [gemini.google.com](https://gemini.google.com)           |
| **DeepSeek**   | DeepSeek (چین)   | [chat.deepseek.com](https://chat.deepseek.com)           |
| **Grok**       | xAI              | [grok.com](https://grok.com)                             |
| **GLM (Z.AI)** | Zhipu AI (چین)   | [z.ai](https://z.ai)                                     |
|                |

---

## مدل‌ها و بنچمارک‌ها (اکتبر ۲۰۲۶)
| دسته مدل | مدل‌های منتخب | مرجع بنچمارک |
| :--- | :--- | :--- |
| **مدل‌های زبانی** | GPT-6, Gemini 4 Pro, Claude Opus 5.5, Grok 4.7 | [LMArena](https://arena.ai), [Artificial Analysis](https://artificialanalysis.ai/) |
| **متن به تصویر** | Nano Banana Pro, FLUX 2, Imagen 4 | [Artificial Analysis](https://artificialanalysis.ai/models/text-to-image) |
| **توصیف تصویر** | Florence-2, Qwen2-VL | [OpenVLM Leaderboard](https://huggingface.co/spaces/opencompass/open_vlm_leaderboard) |
| **متن به ویدئو** | Runway Gen-3, Kling AI | [Video Gen Leaderboard](https://huggingface.co/spaces/ArtificialAnalysis/Video-Generation-Leaderboard) |
| **مدل‌های چندوجهی** | GPT-6, Gemini 4 | [MMMU Benchmark](https://mmmu-benchmark.github.io/) |
| **بینایی-زبانی** | InternVL2, Qwen2-VL | [OpenCompass](https://huggingface.co/spaces/opencompass/open_vlm_leaderboard) |
| **تخصصی (ریاضی/کد)** | Claude Opus 5.5, DeepSeek V4.1 | [Epoch AI](https://epoch.ai/frontiermath), [LiveCodeBench](https://livecodebench.github.io/leaderboard.html) |

<!-- ---

![bg](img/gemini-limit.png) -->

---

![bg](img/LLM-comparing-Dec-2025.png)

######[AI model Grok 4.2 wins Alpha Arena trading tournament](https://forklog.com/en/ai-model-grok-4-2-triumphs-in-trading-tournament/)

*تصویر آرشیوی ۲۰۲۵ — وضعیت روز را در [llm-stats](https://llm-stats.com/) ببینید*

---

![bg opacity:0.85](img/llm-stats.png)

### [llm-stats.com: AI Leaderboards](https://llm-stats.com/)

### [llm-stats.com: Benchmarks](https://llm-stats.com/benchmarks)

---

![bg opacity:0.25](img/text-to-text-bg.png)

### مدل‌های «تولید متن از متن» (Text → Text)

| نمونه                                              | کاربرد اصلی                   | مالک      |
| -------------------------------------------------- | ----------------------------- | --------- |
| [ChatGPT](https://chatgpt.com)                     | گفتگو، کدنویسی، نگارش علمی    | OpenAI    |
| [Claude](https://claude.ai)                        | تحلیل عمیق، استدلال متنی      | Anthropic |
| [Gemini](https://gemini.google.com)                | چندوجهی، جستجوی هوشمند        | Google    |
| [DeepSeek](https://chat.deepseek.com)              | استدلال و کدنویسی             | DeepSeek  |
| [Microsoft Copilot](https://copilot.microsoft.com) | دستیار برنامه‌نویسی و آفیس    | Microsoft |
| [Grok](https://grok.com)                           | گفتگو با دسترسی به داده‌های X | xAI       |
| [GLM (Z.AI)](https://z.ai)                         | کدنویسی و وظایف تخصصی         | Zhipu AI  |

> این گروه، ستون فقرات ابزارهای پژوهشی مبتنی بر LLM محسوب می‌شود.

---

![bg opacity:0.2](img/text-to-image-bg.png)

## تولید تصویر از متن — (Text → Image)

| ابزار                                         | کاربرد / ویژگی                           |
| --------------------------------------------- | ---------------------------------------- |
| [Imagine.art](https://www.imagine.art)        | تولید تصویر فوری، رایگان، مدل‌های تعاملی |
| [Text to Image](https://www.texttoimage.org/) | رایگان                                   |
| [Canva AI](https://www.canva.com)             | تولید سریع تصویر + ابزار طراحی           |
| [Leonardo AI](https://www.leonardo.ai)        | تصویرسازی هنری / مفهومی                  |
| [Dream by Wombo](https://dream.ai/)           | تولید تصویر با سبک‌های هنری              |

---

یک متن فارسی در مورد ترکیبی از خصوصیات سه تن از اساتید را به کوپایلوت دادم و پرامپت مناسب به زبان انگلیسی خواستم که این شد:

###### A cheerful middle-aged professor (around 45 years old) with short beard and salt-and-pepper hair, smiling warmly in his office at Ferdowsi University of Mashhad. His office is decorated with Tintin posters, figurines, and memorabilia, along with many flowers and green plants. A large glass blackboard, gifted by his students, is mounted on the wall, covered with colorful mathematical formulas written in marker. Several students are gathered around him, engaged in lively discussion, showing their admiration for his love of teaching. The office also contains a sofa, desk, chairs, computer, and coffee, creating a cozy and intellectual atmosphere full of energy and inspiration.

---

## خروجی کوپایلوت با GPT-5

![bg opacity:0.8](img/Copilot_GPT5.jpg)

---

## خروجی imagine.art با Nano-Banana-Pro

![bg opacity:0.8](img/imagine.art-Nano-Banana-Pro_A_cheerful_middle-aged_professor.jpg)

---

![bg right opacity:0.8](img/NST-Amintoosi.png)

 <!-- مقایسه دو ابزار رایگان تولید تصویر با AI -->

- GPT-5 vs Nano Banana Pro
- تفاوت در واقع‌گرایی، وضوح، سبک هنری
- مناسب برای کدام کاربرد؟ (پوستر، ارائه، مقاله، تصویرسازی مفهومی)
- برای اطلاعات بیشتر در مورد شیوه تقلید یک اثر هنری در نقاشی ارائه‌ی قبلی با عنوان [انتقال سبک عصبی](https://1drv.ms/p/c/31166a0f5c94f268/EWjylFwPahYggDGCUwAAAAAB8JI2ARAES9QukZKKiM_EHw?e=qsdToe) را ملاحظه فرمایید

---

![bg width:90%](img/ChatGPT-limit.png)

---

## تبدیل تصویر به تصویر (Image → Image)

![bg right](img/mAmintoosi-50.jpg)
![bg right](img/Copilot_Mahmood.jpg)

| ابزار                                                          | کاربرد / ویژگی                            |
| -------------------------------------------------------------- | ----------------------------------------- |
| [Fotor AI](https://www.fotor.com/features/ai-image-generator/) | روتوش، حذف اشیاء، تبدیل سبک عکس           |
| [Photopea](https://www.photopea.com)                           | ویرایشگر آنلاین رایگان با فیلترهای هوشمند |
| [Canva AI](https://www.canva.com)                              | تغییر خودکار سبک، پس‌زمینه، رنگ‌ها        |
| [Pixlr AI](https://pixlr.com)                                  | اصلاح و انتقال سبک                        |

<!-- > این ابزارها برای ترمیم، تغییر سبک و بهبود کیفیت تصاویر موجود مناسب‌اند. -->

---

![bg opacity:0.2](img/one-year-fall-scene.jpg)

## تولید ویدئو از متن (Text → Video)

| ابزار                                                        | کاربرد / ویژگی                                     |
| ------------------------------------------------------------ | -------------------------------------------------- |
| [MovieFlow](https://movieflow.ai/signup?inviteCode=ZCKDT14H) | تولید ویدئوهای کوتاه با استایل سینمایی، پلن رایگان |
| [Hailuo AI Video](https://hailuoai.video/)                   | تولید سریع ویدئو از متن، نسخه رایگان دارد          |
| [Luma AI (Dream Machine)](https://lumalabs.ai/dream-machine) | حرکت طبیعی دوربین و اجسام، نسخه رایگان محدود       |
| [Runway Gen-4](https://runwayml.com) | تولید ویدئو از متن/عکس، نسخه رایگان محدود |
| [Pika](https://www.pika.art)                                 | ویدئوهای کوتاه خلاقانه، پلن رایگان                 |
| [Kapwing AI Video](https://www.kapwing.com/ai)               | ساخت کلیپ از متن، ابزارهای ویرایش رایگان           |

> عمر ابزارها کوتاه است — نمونه: Sora که پارسال در بیسیک جدول‌ها بود، در ۲۰۲۶ تعطیل شد.

---

<!-- html -->
<div style="
  display: flex;
  gap: 30px;
  justify-content: center;
  align-items: center;
  height: 70vh;
">
  
  <div style="width: 25%; text-align: center;">
  <h3>
    برای تولید ویدئو با استفاده از مدلهای زبانی    <a href="https://grok.com/share/c2hhcmQtMg_729a6609-5444-47b6-8619-9c8db0d3b5a3">  سناریو </a>     نوشته شود
    </h3>
    </div>
  <div style="width: 70%; text-align: center;">
    <video 
      autoplay 
      loop 
      muted 
      controls
      style="
        width: 100%;
        height: 60vh;
        border-radius: 10px;
        box-shadow: 0 5px 15px rgba(0,0,0,0.2);
      ">
      <source src="img/one-year.mp4" type="video/mp4">
    </video>
  </div>
</div>

---

<!-- ![bg opacity:0.25](img/multimodal-models-bg.jpg) -->

## مدل‌های چندوجهی — Multimodal AI Models

### ورودی/خروجی: متن، تصویر، صوت، ویدئو

| مدل                                                      | توانایی / ویژگی کلیدی                        |
| -------------------------------------------------------- | -------------------------------------------- |
| [GPT](https://chatgpt.com)                               | متن + تصویر + صوت؛ مکالمه چندحالته           |
| [Gemini](https://gemini.google.com)                      | پردازش متن، تصویر، صوت و ویدئو در مقیاس بزرگ |
| [Claude](https://claude.ai)                              | تحلیل متن و تصویر با دقت بالا                |
| [Ollama Models](https://ollama.com/library)              | اجرای مدل‌های متن‌باز (LLM / VLM) روی لپ‌تاپ |
| [HuggingFace Multimodal](https://huggingface.co/unsloth) | مجموعه‌ای از مدل‌های رایگان متن-باز          |

مقاله با عنوان [The Llama 3 Herd of Models](https://arxiv.org/abs/2407.21783) حدود پانصد نویسنده دارد!

<!-- > مدل‌های چندوجهی مسیر حرکت به سوی [هوش جامع مصنوعی](https://fa.wikipedia.org/wiki/%D9%87%D9%88%D8%B4_%D8%AC%D8%A7%D9%85%D8%B9_%D9%85%D8%B5%D9%86%D9%88%D8%B9%DB%8C) (AGI-like) را نشان می‌دهند. -->

---

## سه لایه ابزار هوش مصنوعی

| لایه                    | چیست؟                                                    | نمونه ابزارها                             |
| ----------------------- | -------------------------------------------------------- | ----------------------------------------- |
| ۱. دستیار گفتگویی       | پاسخ‌ساز؛ ایده و متن از صفر تا یک                        | ChatGPT، Gemini، DeepSeek                 |
| ۲. دستیار مبتنی بر منبع | جستجو در پایگاه‌های واقعی + تحلیل                        | SciNiTO، Elicit، NotebookLM               |
| ۳. عامل (Agent)         | کل پروژه را می‌خواند، کد می‌نویسد، اجرا و بازبینی می‌کند | Freebuff، Copilot، Cursor، Claude Code    |

### نکته کلیدی

> لایه ۱ و ۲ «ایده می‌دهند»، لایه ۳ «کار انجام می‌دهد» — و همان‌جا مسئولیت درستی خروجی بر عهده شماست.

---


## از ایران چه چیزی در دسترس است؟

| وضعیت                                 | نمونه‌ها                             | یادآوری                                     |
| ------------------------------------- | ------------------------------------ | ------------------------------------------- |
| عملاً در دسترس (بومی)                 | SciNiTO، سامانه‌های علمی داخل کشور  | برای پژوهش فارسی نقطه شروع خوبی است        |
| نیازمند IP خارجی و حساب بین‌المللی    | ChatGPT، NotebookLM، عامل‌های ابری   | ثبت‌نام و پرداخت؛ همیشه احتمال محدودیت     |
| متغیر — گاهی مسدود                    | Gemini و سرویس‌های در حال تغییر      | «رایگان بودن» را نزدیک روز کارگاه تست کنید |

### قاعده کارگاه

> هیچ ادعایی درباره دسترسی و رایگان بودن را بدون تست زنده نگویید.

---


![bg opacity:0.22](img/ai-agents-bg.jpg)

## Agentهای هوش مصنوعی چیستند؟

| ویژگی                | توضیح                                                                               |
| -------------------- | ----------------------------------------------------------------------------------- |
| **تعریف**            | سیستم‌هایی که با استفاده از LLM + ابزار + حافظه، وظایف چندمرحله‌ای را انجام می‌دهند |
| **تفاوت با Chatbot** | فقط پاسخ نمی‌دهند؛ برنامه‌ریزی، اجرا و بازبینی می‌کنند                              |
| **کاربردها**         | اجرای pipeline پژوهش، توسعه نرم‌افزار، جستجو و تحلیل خودکار                         |

---

### نمونه Agentها و چارچوب‌ها

- [Freebuff](https://freebuff.com) — عامل کدنویسی که همین ارائه را هم می‌تواند ویرایش کند
- [Copilot / Cursor / Claude Code](https://github.com/features/copilot) — عامل درون ادیتور
- [LangChain](https://www.langchain.com) — چارچوب ساخت عامل اختصاصی

### نکته مهم

> **Agentها قدرتمندند، اما خودمختارِ قابل‌اعتماد نیستند؛  
> نظارت انسانی همچنان ضروری است.**

<!-- html -->
<div style="
  display: flex;
  gap: 30px;
  justify-content: center;
  align-items: center;
  height: 70vh;
">
  
  <div style="width: 45%; text-align: center;">
    <video 
      autoplay 
      muted 
      controls
      style="
        width: 100%;
        height: 60vh;
        border-radius: 10px;
        box-shadow: 0 5px 15px rgba(0,0,0,0.2);
      ">
      <source src="img/AI_Research_Workflow.mp4" type="video/mp4">
    </video>
    <div style="margin-top: 10px;"><strong>Present</strong></div>
  </div>
    <div style="width: 45%; text-align: center;">
    <video 
      autoplay 
      muted 
      controls
      style="
        width: 100%;
        height: 60vh;
        border-radius: 10px;
        box-shadow: 0 5px 15px rgba(0,0,0,0.2);
      ">
      <source src="img/Academic_Office_Modern_Morph.mp4" type="video/mp4">
    </video>
    <div style="margin-top: 10px;"><strong>  to  </strong></div>
  </div>

  <div style="width: 45%; text-align: center;">
    <video 
      autoplay 
      loop 
      muted 
      controls
      style="
        width: 100%;
        height: 60vh;
        border-radius: 10px;
        box-shadow: 0 5px 15px rgba(0,0,0,0.2);
      ">
      <source src="img/Academic_Seasons_Research_Flow.mp4" type="video/mp4">
    </video>
    <div style="margin-top: 10px;"><strong>From Past</strong></div>
  </div>
</div>

---

<!-- html -->
<div style="
  display: flex;
  gap: 30px;
  justify-content: center;
  align-items: center;
  height: 70vh;
">
  
  <div style="width: 25%; text-align: center;">
    <h2>بخش سوم</h2>
    <h3>
      مهندسی پرامپت: کلید استفاده موثر از مدل‌های هوش مصنوعی
    </h3>
    </div>
  <div style="width: 70%; text-align: center;">
    <video 
      autoplay 
      loop 
      muted 
      controls
      style="
        width: 100%;
        height: 60vh;
        border-radius: 10px;
        box-shadow: 0 5px 15px rgba(0,0,0,0.2);
      ">
      <source src="img/From-Traditional-Research-to AI-Powered-Acceleration.mp4" type="video/mp4">
    </video>
  </div>
</div>

---

## چرا پرامپت‌نویسی مهم است؟

### 🎯 پرامپت = دستورالعمل شما برای AI

- **دقت خروجی:** پرامپت خوب = پاسخ دقیق و مفید
- **کنترل نتیجه:** شما «مهندس» گفتگو هستید
- **بهینه‌سازی:** پرامپت ضعیف = پاسخ بی‌ربط

### [اسلایدهای آماده شده با کمک جمینای ](https://docs.google.com/presentation/d/1IZw3Rj7w47ZrtogpjayEacRhTEoO1YqWHGNgzWMRnjc/edit?usp=sharing)

---

![bg opacity:0.22](img/prompt-framework-bg.jpg)

### چارچوب پرامپت حرفه‌ای

| مؤلفه               | توضیح مختصر             | نمونه                                            |
| ------------------- | ----------------------- | ------------------------------------------------ |
| **Persona (شخصیت)** | تعیین نقش یا تخصص AI    | «تو یک محقق یادگیری ماشین هستی.»                 |
| **Context (زمینه)** | ارائه اطلاعات پیش‌زمینه | «در حال نوشتن بخش کارهای مرتبط درباره CNN هستم.» |
| **Task (وظیفه)**    | مشخص‌کردن کار اصلی      | «۱۰ مقاله کلیدی را فهرست کن.»                    |
| **Format (قالب)**   | شکل خروجی               | «نتیجه را در قالب جدول LaTeX بده.»               |
| **Tone (لحن)**      | سبک و لحن متن           | «لحن رسمی، علمی و دقیق باشد.»                    |
| **Exemplar(نمونه)** | نمونه ورودی/خروجی       | «چند مثال برای تقلید ارائه می‌دهم.»              |

> ساختاردهی صحیح پرامپت کیفیت خروجی مدل‌های زبانی را چند برابر افزایش می‌دهد.

<!-- ###### Professional Prompt Engineering (P–C–T–F–T–E) -->

---

![bg opacity:0.22](img/prompt-best-practices-bg.jpg)

## نکات کلیدی مهندسی پرامپت

| موضوع                             | نکته کاربردی (خلاصه)                                                               |
| --------------------------------- | ---------------------------------------------------------------------------------- |
| **مرحله‌به‌مرحله (Step-by-step)** | خروجی را گام به گام بخواهید                                                        |
| **جداکننده‌ها (Delimiters)**      | برای مشخص‌کردن متن هدف از جداکننده سه‌گانه استفاده کنید: <br>`"""متن شما اینجا"""` |
| **Few-shot (نمونه‌های آموزشی)**   | چند مثال مطلوب نشان بدهید تا قالب موردنظر را یاد بگیرد. (۲–۳ مثال کافی است)        |
| **توسعه تکراری (Iterate)**        | پرامپت را اجرا کن ← خروجی را آنالیز کن ← پرامپت را اصلاح کن ← مجدداً اجرا کن.      |

---

![bg opacity:0.2](img/simulation.jpg)

⭐ تکنیک شبیه‌سازی: (برگرفته از [کانال هوش‌مصنوعی در پژوهش،](http://t.me/ai_in_research))

چرا فقط درباره «مصاحبه کاری» یا «دفاع پایان‌نامه» سوال می‌پرسی وقتی می‌تونی واقعاً تجربه‌ش کنی؟ 😎

🔵 تکنیک «شبیه‌سازی» (Simulation)، هوش مصنوعی رو از یه «موتور جستجو» تبدیل می‌کنه به یه «شبیه ساز تمرینی»

به جای اینکه لیست سوالات رو بگیری، بهش بگو محیط رو برات بازسازی کنه! بهش بگو نقش طرف مقابل (استاد راهنما، مشتری عصبانی، مصاحبه‌گر گوگل) رو بازی کنه و یکی‌یکی ازت سوال بپرسه.

<!-- ❌ روش غلط (متنی):
«سوالات رایج در جلسه دفاع پایان‌نامه ارشد روانشناسی چیست؟» (نتیجه: یه لیست خشک و خالی که فقط می‌خونی.) -->

✅ مثال:
«می‌خواهم جلسه دفاع پایان‌نامه‌ام را تمرین کنم. تو نقش "استاد داور سخت‌گیر" را بازی کن. موضوع من "هوش مصنوعی در روانشناسی" است. جلسه را شروع کن و سوالات را دانه دانه از من بپرس و منتظر جوابم بمان. بعد از هر جواب، نظر بده و سوال بعدی را بپرس.»

مأخذ ایده: [کانال هوش‌مصنوعی در پژوهش](http://t.me/ai_in_research)

---

# بخش آموزش

> تکلیف‌هایی که «محصول نهایی» است، امروز عامل‌های AI می‌توانند کامل تحویل بدهند؛ ارزیابی ما باید بازطراحی شود.

---


## AI در آموزش: از کجا شروع کنیم؟

| کاربرد                       | مثال عملی                                                                       |
| ---------------------------- | ------------------------------------------------------------------------------- |
| طراحی سؤال و آزمون           | تولید سؤال چندگزینه‌ای از جزوه + بازبینی انسانی                                 |
| ساخت روبریک و معیار نمره‌دهی | تبدیل سرفصل درس به روبریک شفاف                                                 |
| بازخورد سریع روی پیش‌نویس    | «برای این درس نقد مفهومی بده، نه درست‌نویسی املایی»                             |
| ارائه و پادکست درسی          | تبدیل جزوه به خلاصه صوتی برای مرور (NotebookLM — از ایران گاهی محدود)           |
| بازطراحی تکلیف               | تمرکز از «محصول نهایی» به «فرایند کار»                                          |

---


## بازطراحی تکلیف: محصول یا فرایند؟

| به‌جای این معیار                    | این نشانه‌های فرایند را بسنجید                        |
| ----------------------------------- | ------------------------------------------------------ |
| فقط فایل نهایی گزارش                | نسخه میانی + دفاع حضوری کوتاه                          |
| پروژه بدون همراهی                   | توضیح کتبی و گفتگوی کوتاه درباره تصمیم‌ها              |
| آزمون انجام‌شده در خانه             | آزمون کوتاه حضوری                                     |

- بخشی از نمره برای «توضیح قدم‌ها و انتخاب‌ها»
- تکلیف پیشنهادی: «بخشی از گزارش که با AI ساختی را علامت بزن و تبیین کن چرا آن را نگه داشتی و کجا را اصلاح کردی»

---


## دتکتورهای هوش مصنوعی: قابل اعتماد نیستند

- **خطای مثبت کاذب:** حتی خطای حدود ۱ درصد، در مقیاس یک دانشگاه یعنی صدها هشدار اشتباه
- **دور زدن آسان:** یک بازنویسی ساده کافی است تا نتیجه دتکتور تغییر کند
- **واکنش مراکز:** بسیاری از دانشگاه‌ها استفاده از دتکتور برای حکم‌گذاری را متوقف کرده‌اند
- **پیام کارگاه:**

> دتکتور «مدرک» نیست؛ فقط «قرینه» است — مبنای تصمیم را بازطراحی تکلیف و نشانه‌های فرایند بگذارید.

---


## وضعیت جهانی (اکتبر ۲۰۲۶)

| یافته                                                          | اهمیت برای کلاس                                            |
| -------------------------------------------------------------- | ---------------------------------------------------------- |
| اکثریت قاطع اعضای هیأت علمی از AI استفاده می‌کنند (یونسکو)     | «ممنوع کردن کامل» عملاً ممکن نیست                          |
| بخش کوچکی از دانشگاه‌ها سیاست مصوب دارند؛ بقیه در حال تدوین‌اند | سیاست کلاسی خود را همین امسال مشخص کنید                    |
| برخی مراکز دتکتورها را از ارزیابی خارج کرده‌اند                | ارزیابی بر مبنای فرایند و گواهی حضوری جایگزین می‌شود       |

---


## سیاست اعلام استفاده در کلاس — نمونه اعلام

> «می‌توانید از ابزارهای مولد استفاده کنید، اگر: (۱) کجا و چگونه از آن‌ها استفاده کردید را به‌طور خلاصه اعلام کنید، (۲) همه ادعاها و منابع را راستی‌آزمایی کنید، (۳) در صورت پرسیدن بتوانید هر پاراگراف را خودتان تبیین کنید.»

- نسخه «تا اطلاع ثانوی غیرفعال» هم مجاز است؛ اما چرایی آن را توضیح دهید
- برای هر تکلیف از ابتدا مشخص کنید: «با AI چه چیزهایی مجاز است و چه چیزی نه»

---


![bg opacity:0.8](img/Exam-Generation.png)

## [سامانه ](https://github.com/sirnaser/modern-qg) طرح سؤال از مطالب درسی

---

# نشست ۲

## پژوهش در عصر هوش مصنوعی

---


![bg opacity:0.3](img/GenAI_tool_map_Aug_2025_v2.jpg)

# بخش دوم

## [ابزارهای هوش مصنوعی برای پژوهش](https://libguides.lib.hku.hk/AI-literacy/GenAI4Education)

---

## ابزارهای هوش مصنوعی برای پژوهش علمی

### از جستجو تا مستندسازی و نگارش مقاله

| ابزار                                                | کاربرد اصلی                                          |
| ---------------------------------------------------- | ---------------------------------------------------- |
| [SciNiTO](https://scinito.ai/)                       | جست‌وجوی دقیق علمی، یافتن مقالات مرتبط               |
| [NotebookLM](https://notebooklm.google.com/)         | ساخت مدل زبانی اختصاصی از PDFها و یادداشت‌های پژوهشی |
| [Gemini](https://gemini.google.com/)                 | تحلیل فایل‌های PDF، استدلال علمی، جستجو              |
| [Connected Papers](https://www.connectedpapers.com/) | شبکه استنادی و یافتن مقاله‌های مشابه                 |
| [Elicit](https://elicit.com/)                        | مرور ادبیات (Literature Review) نیمه‌خودکار          |

> این ابزارها چرخه پژوهش—from idea to publication—را سرعت می‌بخشند.

---

![bg](img/scinito-AI.png)

[UM Library](https://library.um.ac.ir/index.php/fa/news-archive-fa/scinito-videos)

[SciNiTO](https://www.scinito.ai/)

---

<!-- html -->
<div style="
  display: flex;
  justify-content: center;
  align-items: center;
  height: 80vh; /* یا 85vh */
  margin: 0 auto;
">
  <div style="
    width: 80%; /* یا 80% */
    text-align: center;
  ">
    <video 
      controls 
      style="
        width: 100%;
        height: 70vh; 
        border-radius: 12px;
        box-shadow: 0 6px 20px rgba(0,0,0,0.25);
        background: #000; 
        object-fit: contain; 
      ">
      <source src="https://library.um.ac.ir/images/Education/Tutorial_Videos/SCINITOAI/SCiNiTO%20AI-5%20Research%20Chatbot.mp4" type="video/mp4">
      مرورگر شما از تگ ویدئو پشتیبانی نمی‌کند.
    </video>
  </div>
</div>

---

![bg opacity:0.22](img/ai-research-workflow-bg.jpg)

## چرخه پژوهش با کمک هوش مصنوعی

<!-- ### Research Workflow with AI -->

| مرحله                        | نقش AI                                                |
| ---------------------------- | ----------------------------------------------------- |
| **۱. ایده‌پردازی**           | یافتن سؤال پژوهشی، بررسی امکان‌پذیری، تولید فرضیه     |
| **۲. جستجوی ادبیات**         | یافتن مقالات کلیدی، گراف استنادی، استخراج شکاف پژوهشی |
| **۳. طراحی آزمایش**          | پیشنهاد روش، تولید کد اولیه، طراحی پروتکل آزمایشی     |
| **۴. تحلیل داده**            | اجرای کد، مصورسازی، تحلیل آماری و مدل‌سازی            |
| **۵. نگارش مقاله**           | نوشتن مقدمه، روش، نتایج، خلاصه‌سازی کل مقاله          |
| **۶. بازبینی علمی**          | نقد بخش‌های مقاله، رفع ابهام، بررسی دستور زبان و منطق |
| **۷. آماده‌سازی برای ارسال** | فرمت‌بندی، تولید کاورلتر، بهبود شکل‌ها                |
| **۸. پاسخ به داوران**        | اصلاح مقاله و آماده‌سازی فایل پاسخ به داوران          |

> AI یک دستیار چند مرحله‌ای در کل فرایند پژوهش است؛ از آغاز تا انتها.

---

![bg opacity:0.25](img/ai-litreview-bg.jpg)

## جستجوی ادبیات با ابزارهای هوشمند

### AI-Assisted Literature Review

### ابزارهای اصلی

- **[SciNiTO](https://scinito.ai/)** – جست‌وجوی دقیق علمی، یافتن مقالات مرتبط بر اساس مفهوم
- **[Connected Papers](https://www.connectedpapers.com/)** – تولید گراف استنادی و تشخیص «مقالات مرتبط»
- **[Elicit](https://elicit.com/)** – مرور ادبیات نیمه‌خودکار با ترکیب LLM و پایگاه‌های واقعی
- **[NotebookLM](https://notebooklm.google.com/)** – ساخت دستیار پژوهشی اختصاصی از چند PDF و یادداشت
  - استفاده از NotebookLM‌ در ایجاد پادکست [درس داده‌کاوی](https://fum-cs.github.io/data-mining/intro.html)

<!-- ### کاربردها

- یافتن مقالات کلیدی (Anchor Papers)
- شناسایی شکاف پژوهشی (Research Gap)
- ساخت گراف ساختار دانش (Knowledge Graph)
- خلاصه‌سازی چندمقاله‌ای و استخراج الگوها

> مرور ادبیات با AI از یک فرآیند چندروزه به یک کار چندساعته تبدیل می‌شود. -->

---

![bg](img/jupyter-book-tutorial.png)

### [آشنایی با Jupyter-Book](https://fum-cs.github.io/jupyter-book-tutorial/docs/home.html)

---

| فرمت / سامانه           | SEO        | LLM        |
| ----------------------- | ---------- | ---------- |
| HTML استاتیک            | عالی       | عالی       |
| RevealJS / Marp HTML    | عالی       | عالی       |
| Hugo / MkDocs / Alfolio | عالی       | عالی       |
| PDF در سایت عمومی       | متوسط      | متوسط      |
| Google Slides (عمومی)   | ضعیف       | ضعیف       |
| Dropbox PDF             | بسیار ضعیف | بسیار ضعیف |
| OneDrive PPT/PDF        | بسیار ضعیف | بسیار ضعیف |
| Moodle / LMS دانشگاهی   | بسیار ضعیف | بسیار ضعیف |

تفاوت روشهای مختلف نشر دانش در دیده شدن

---

## دستیارهای «پژوهش عمیق» (Deep Research)

| ابزار                       | چه می‌کند                              | نکته دسترسی                       |
| --------------------------- | -------------------------------------- | --------------------------------- |
| SciNiTO / Elicit            | منابع واقعی با DOI/PMID و تحلیل       | برای پژوهش علمی، شروع بهتر        |
| NotebookLM                  | مرور اسناد خودشما و ساخت گزارش        | از ایران گاهی محدود است           |
| ChatGPT / Gemini Deep Research | دامنه‌دار، مرور سریع موضوع          | نیازمند IP خارجی                  |
| Perplexity                  | منابع زنده همراه پاسخ                 | نسخه رایگان محدود                 |

### قاعده

> خروجی فقط نقطه شروع است؛ هر ادعا را با اصل منبع (DOI/PMID) راستی‌آزمایی کنید.

---


<!-- مشکل اصلی با ابزارهای هوش مصنوعی: **عدم قطعیت**!!! -->

![bg opacity:0.2](img/ai-uncertainty-bg.jpg)

## عدم قطعیت در مدل‌های مولد هوش مصنوعی

| واقعیت فنی              | توضیح کوتاه                                     | پیام برای پژوهشگر              |
| ----------------------- | ----------------------------------------------- | ------------------------------ |
| **ماهیت احتمالی**       | خروجی‌ها بر اساس احتمال تولید می‌شوند، نه قطعیت | پاسخ‌ها می‌توانند متفاوت باشند |
| **عدم حقیقت‌سنجی ذاتی** | هدف مدل تولید متن محتمل است، نه صحت علمی        | امکان پاسخ قانع‌کننده ولی غلط  |
| **عدم درک نیت واقعی**   | مدل فقط پرامپت را تفسیر آماری می‌کند            | نیاز به مهندسی پرامپت دقیق     |
| **توهم‌زایی**           | امکان ساخت منبع، عدد یا ادعا                    | ممنوع برای استناد مستقیم       |

**خروجی AI باید همیشه راستی‌آزمایی شود، به‌ویژه در مقاله علمی**

<!-- ### به نتایج هیچ کدام نمی‌توان اطمینان صددرصد درست داشت!!

### یا آنچه می‌خواهیم را نمی‌دهند! -->

---

![bg opacity:0.2](img/ai-what-it-doesnt-understand-bg.jpg)

<!-- html -->
<style>
.small-text {
  font-size: 0.8em !important;
  line-height: 1.4 !important;
}
.compact-list li {
  margin-bottom: 5px !important;
}
</style>

<div style="
  height: 90vh;
  padding: 10px;
  overflow-y: auto;
  border-radius: 8px;
  box-shadow: inset 0 0 10px rgba(0,0,0,0.05);
" class="small-text">

### AI چه چیزی را نمی‌فهمد؟

| محدودیت بنیادی        | توضیح کوتاه                                                    | پیام برای پژوهش                    |
| --------------------- | -------------------------------------------------------------- | ---------------------------------- |
| **عدم فهم حقیقت**     | مدل‌ها حقیقت‌سنج یا علّی نیستند؛ الگوهای زبانی را یاد می‌گیرند | نتایج نیازمند داوری انسانی         |
| **عدم فهم «نبودن»**   | آنچه در داده‌ها نیست، به‌صورت صریح مدل نمی‌شود                 | سکوت داده ≠ نفی علمی               |
| **عدم کشف بدون داده** | کشف مفاهیم خارج از توزیع آموزشی ممکن نیست                      | انتظار «نبوغ اکتشافی» نداشته باشید |
| **عدم نیت و هدف**     | مدل هدف علمی ندارد؛ فقط پاسخ محتمل می‌دهد                      | مسئولیت تفسیر با پژوهشگر است       |

### پیام کلیدی

> **AI آنچه را دیده و آموخته بازترکیب می‌کند؛  
> فهم، نفی، و کشفِ بنیادی وظیفه انسان است.**

</div>

---

![bg opacity:.3](img/Soltan-Mahmood.webp)

## من ندیم توام نه ندیم بادمجان

«سلطان محمود» را در هنگام گرسنگی «بادمجان بورانی» پیش آوردند، خوشش آمد و گفت: بادمجان طعامی است خوش.
ندیمی در مدح بادمجان فصلی پرداخت و [سلطان محمود] چون سیر شد گفت: بادمجان چیز خیلی مضری است.
ندیم، باز در مضرت بادمجان مبالغتی تمام كرد.
سلطان گفت: ای مردک نه این زمان كه مدحش می‌گفتی؟
گفت: من ندیم توام نه ندیم بادمجان، مرا چیزی باید گفت كه تورا خوش آید نه بادمجان را.

عبید زاکانی ـ رساله دلگشا

---

![bg opacity:0.5](img/LLMs-vs-SE.jfif)

## جستجو در موتورهای جستجو و سامانه‌های جدید هوشمند

#### جستجوی عبارت:

### "لیست اعضای هیات علمی گروه علوم کامپیوتر دانشگاه فردوسی مشهد"

---

![bg height:100%](img/CS-Staff-google.png)
![bg height:100%](img/CS-Staff-bing.png)

---

![bg height:100%](img/CS-Staff-microsoft-copilot.png)
![bg height:100%](img/CS-Staff-perplexity.png)

---

![bg height:100%](img/CS-Staff-ChatGPT-1.png)
![bg height:100%](img/CS-Staff-ChatGPT-2.png)

---

![bg height:100%](img/CS-Staff-gemini.png)
![bg height:100%](img/CS-Staff-grok.png)

---

حتی نتایج گوگل هم ممکن است اشتباه باشد!

![](img/ISPRS-google-result.png)

---

|                                              |                                                |
| :------------------------------------------: | :--------------------------------------------: |
| ![](img/ISPRS-ISSN-scimago-impactfactor.png) | ![](img/ISPRS-ISSN-google-kg-impactfactor.png) |

---

### ابزارهای پژوهشی هوشمند چگونه خطای منبع را کاهش می‌دهند؟

![bg opacity:0.2](img/rag-vs-llm-bg.jpg)

| رویکرد           | نحوه کار                                  | میزان اعتماد        |
| ---------------- | ----------------------------------------- | ------------------- |
| **LLM خالص**     | تولید پاسخ صرفاً بر اساس مدل زبانی        | ❌ پایین برای منابع |
| **RAG-based AI** | جستجو در پایگاه داده واقعی + تحلیل با LLM | ✅ بالا برای منابع  |

### معماری ابزارهایی مثل SciNiTO / Elicit

| مرحله    | توضیح                                                       |
| -------- | ----------------------------------------------------------- |
| 1️⃣ جستجو | بازیابی مقاله از پایگاه‌های واقعی (CrossRef, PubMed, arXiv) |
| 2️⃣ فیلتر | انتخاب مقالات مرتبط با DOI و متادیتا                        |
| 3️⃣ تحلیل | خلاصه‌سازی و خوشه‌بندی با LLM                               |
| 4️⃣ ارائه | لینک واقعی، قابل کلیک و بررسی                               |

### نکته کلیدی

> **منابع واقعی‌اند، اما تفسیر آن‌ها همچنان نیازمند قضاوت انسانی است**

---

## چک‌لیست پیش از اعتماد به هر منبع

- DOI/PMID واقعاً وجود دارد؟ (در CrossRef/PubMed جست‌وجو کنید)
- عنوان و نویسنده‌ها با اصل منبع مطابق‌اند؟
- ادعای متن با متن مقاله اصلی یکی است؟
- تفکیک مسئولیت: ابزار بازیابی می‌کند؛ راستی‌آزمایی با شماست.

---


## مطالعه موردی: از مخزن کد تا پیش‌نویس مقاله

> اسکرین‌شات‌ها با Copilot (۲۰۲۵) گرفته شده‌اند — همین گردش کار امروز با Freebuff و هر عامل کدنویسی دیگری تکرارپذیر است.

![bg](img/copilot/01-start.png)

---

# پرامپت اول:

این مخزن شامل برنامه هایی هست که برای بررسی امکان استفاده از «تعبیه سازی گراف» در ارزش گذاری قیمت املاک نوشته ام و بر روی دو مجموعه داده اجرا شده است.
فایل اصلی 'main_pyg.py' هست که در 'main.ipynb'
بر روی مجموعه دادگان مختلف فراخوانی شده و نتایج اجرای قبلی در پوشه
'results-gpu' ذخیره شده است.
ابتدا مخزن را بررسی کن و یک گزارش در مورد روند کار و ورودی ها و خروجی ها بده که مطمئن شوم روال کار را متوجه شده‌ای

---

![bg](img/copilot/02-first-response.png)

---

<!-- html -->
<div style="
  height: 100vh;
  overflow-y: auto;
  padding-right: 10px; /* برای اسکرول بار */
">
  <img 
    src="img/copilot/03-copilot-first-response.png" 
    alt="تصویر با جزئیات"
    style="
      width: 100%;
      height: auto;
      min-height: 4800px;
      object-fit: contain;
    "
  >
</div>

<div style="
  position: fixed;
  bottom: 20px;
  left: 20px;
  background: rgba(0, 122, 204, 0.9);
  color: white;
  padding: 10px 15px;
  border-radius: 8px;
  font-size: 0.9em;
  z-index: 100;
">
  🔽 برای دیدن جزئیات به پایین اسکرول کنید
</div>

---

### پیشنهاد عنوان مقاله

<!-- شما اکنون به کل این مخزن کد دسترسی دارید و ساختار پروژه، هدف آن، روش‌ها و نتایج قابل استخراج از کد را تحلیل کرده‌اید. لطفاً با توجه به محتوای این مخزن، چند عنوان دقیق، فنی، و مناسب برای یک مقاله پژوهشی در حوزه مرتبط پیشنهاد بده. عناوین باید به زبان انگلیسی باشند و بازتاب‌دهنده نوآوری‌ها، هدف پروژه، و روش پیاده‌سازی موجود در این کد باشند. لطفاً 3 تا 5 عنوان پیشنهادی ارائه کن.

--- -->

<!-- html -->
<div style="
  height: 100vh;
  overflow-y: auto;
  padding-right: 10px; /* برای اسکرول بار */
">
  <img 
    src="img/copilot/04-title-suggestion.png" 
    alt="تصویر با جزئیات"
    style="
      width: 100%;
      height: auto;
      min-height: 2500px;
      object-fit: contain;
    "
  >
</div>

<div style="
  position: fixed;
  bottom: 20px;
  left: 20px;
  background: rgba(0, 122, 204, 0.9);
  color: white;
  padding: 10px 15px;
  border-radius: 8px;
  font-size: 0.9em;
  z-index: 100;
">
  🔽 برای دیدن جزئیات به پایین اسکرول کنید
</div>

---

<!-- html -->
<style>
.tiny-text {
  font-size: 0.7em !important;
  line-height: 1.4 !important;
}
.compact-list li {
  margin-bottom: 5px !important;
}
</style>

<div style="
  height: 90vh;
  padding: 10px;
  overflow-y: auto;
  border-radius: 8px;
  box-shadow: inset 0 0 10px rgba(0,0,0,0.05);
" class="tiny-text">
 عنوان 2 را انتخاب  می کنم، لطفاً یک درفت اولیه با لاتک از یک مقاله پژوهشی به زبان انگلیسی تولید کن.

- مشخصات نویسنده:‌ Mahmood Amintoosi,
  Ferdowsi University of Mashhad, Computer Science Dept.

- ساختار مقاله باید شامل بخش‌های زیر باشد:

1. Abstract 2. Introduction 3. Proposed Method 4. Experimental Results

- متن مقاله رسمی، آکادمیک، و استاندارد باشد. از محتواهای موجود در کد، فایل‌ها، ساختار پروژه، منطق پیاده‌سازی، و نوآوری‌های آن برای نوشتن مقاله استفاده کن. در صورت لزوم، معماری یا روش‌ها را به‌صورت منسجم بازنویسی کن تا متن مقاله روان و علمی باشد.

- فایلهای نتایج - تصاویر و فایلهای لاتک جداول مقایسات - در پوشه 'results-gpu' موجود است.

- یک پوشه با نام docs ایجاد کن و فایل لاتک مقاله به همراه فایلهای احتمالی مورد نیاز را در آن قرار بده.

- پیشنهاد می کنم به نتایج تولید شده در همان مسیرها که هستند لینک بدهی که در صورت اجرای مجدد، با پردازش مجدد فایل لاتک، نتایج جدید در مقاله قرار داده شوند.

- هدف من آموزشی است، بنابراین نیازی به ارائه جزئیات بسیار پیچیده نیست؛ فقط یک پیش‌نویس منظم، حرفه‌ای، و آکادمیک ارائه بده.

- بعد از نوشتن مقاله، pdflatex را روی سند اجرا کن (در مسیر سیستم من هست).
</div>

---

![bg](img/copilot/05-creating-paper.png)

---

![bg](img/copilot/06-created-paper-page1.png)

---

![bg](img/copilot/07-created-paper-page2.png)

---

یک مجله مناسب برای ارسال
این مقاله پیشنهاد بده و یک
Cover Letter
برای آن در قالب لاتک آماده کن.

![bg](img/copilot/08-cover-letter.png)

---

![bg](img/copilot/09-two-comments.png)

---

![bg](img/copilot/10-revised-paper.png)

---

![bg opacity:0.2](img/Kevin-Zhu-NeurIPS-2025.png)

## مثلا ما خوشحالیم که مقاله آماده شد 😃

اما

- نظراتی که برای داور نوشته همون نظرات داور نیستند!
- نمی‌توانیم مطمئن باشیم که بخشهای اصلی مقاله خراب نشده باشند!
- ملت دارن با سرعت مقاله می‌نویسن و حتما در صفی طولانی قرار خواهیم گرفت!
  - [Kevin Zhu](https://neurips.cc/virtual/2025/search?query=Kevin+Zhu)

---

![bg opacity:0.18](img/ai-ethics-bg.jpg)

## چالش‌ها و ملاحظات اخلاقی در استفاده از هوش مصنوعی

<!-- html -->
<style>
.tiny-text {
  font-size: 0.9em !important;
  line-height: 1.1 !important;
}
.compact-list li {
  margin-bottom: 5px !important;
}
</style>

<div style="
  height: 90vh;
  padding: 10px;
  overflow-y: auto;
  border-radius: 8px;
  box-shadow: inset 0 0 10px rgba(0,0,0,0.05);
" class="tiny-text">

| چالش                          | توضیح مختصر                                 | راه‌حل‌های کلیدی                                                    |
| ----------------------------- | ------------------------------------------- | ------------------------------------------------------------------- |
| **توهم‌زایی (Hallucination)** | تولید اطلاعات ساختگی، ارجاعات و آمار نادرست | راستی‌آزمایی، تطبیق چندمنبعی، درخواست شفاف‌سازی از مدل              |
| **سوگیری (Bias)**             | بازتاب سوگیری موجود در داده‌های آموزشی      | استفاده از چند مدل، بررسی خروجی، تنظیم دقیق درخواست                 |
| **عدم تبیین‌پذیری**           | فرایند تصمیم‌گیری مدل روشن نیست             | ساده‌سازی مسئله، تست سناریوها، استفاده از مدل‌های قابل‌توضیح‌تر     |
| **محرمانگی داده**             | احتمال نشت اطلاعات حساس                     | حذف داده شخصی، فعال‌سازی حالت Private، استفاده از نسخه‌های محلی     |
| **وابستگی بیش‌ازحد**          | تضعیف مهارت تحلیل و تفکر پژوهشگر            | استفاده تکمیلی (نه جایگزین)، بازنگری انسانی، مستندسازی              |
| **مالکیت فکری و انتساب**      | ابهام در اینکه چه چیزی «اثر شما» است        | ذکر استفاده از AI، ذخیره نسخه‌های میانی، بررسی محدودیت‌های کپی‌رایت |

</div>

---

## سیاست ناشران در برابر هوش مصنوعی

| قاعده رایج در ناشران بزرگ                   | توضیح                                                         |
| ------------------------------------------- | ------------------------------------------------------------- |
| AI نمی‌تواند نویسنده باشد                   | مسئولیت کامل محتوا بر عهده نویسندگان است                     |
| استفاده از AI باید اعلام شود                | عملاً در فرم ارسال مقاله                                     |
| کاربرد در مرحله روش پژوهش                   | باید در بخش Methods توضیح داده شود                           |
| تصاویر AI عموماً محدود/ممنوع                | به‌ویژه به‌جای شکل تحلیلی یا کاور مقاله                       |
| مسئولیت صحت همه اجزا با نویسندگان           | «ابزار مجاز است، خروجیِ راستی‌آزمایی‌نشده مجاز نیست»          |

---


## منابع ساختگی: یک روند نگران‌کننده

| سال    | از هر N مقاله‌ی فهرست‌شده در PubMed که منباعِ مجعول دارد |
| ------ | ---------------------------------------------------------- |
| ۲۰۲۳   | حدود ۱ در ۲٬۸۲۸                                           |
| ۲۰۲۵   | حدود ۱ در ۴۵۸                                             |
| ۲۰۲۶   | حدود ۱ در ۲۷۷ — تقریباً ده‌برابر سریع‌تر از سه سال پیش    |

### نمونه

> بازپس‌گیری سال ۲۰۲۶ نامه‌ای علمی: از ۱۵ منبع ذکرشده، دست‌کم ۱۰ منبع اصلاً وجود نداشت.

- مأخذ: [Retraction Watch، مه ۲۰۲۶](https://retractionwatch.com/2026/05/07/one-in-277-pubmed-indexed-papers-in-2026-shows-fabricated-references-says-analysis/)

---


![bg opacity:0.2](img/ai-summary-bg.jpg)

## جمع‌بندی

| نکته                                    | توصیه عملی                                                    |
| --------------------------------------- | ------------------------------------------------------------- |
| **AI ابزار قدرتمند است، نه جایگزین ما** | از آن برای سرعت و کیفیت استفاده کنید، نه برای حذف تفکر انسانی |
| **اهمیت کلیدی مهندسی پرامپت**           | پرسونا + زمینه + وظیفه + قالب ← خروجی بهتر                    |
| **فرصت‌های گسترده**                     | کدنویسی، تحلیل داده، نگارش، کاوش ادبیات، تولید ایده           |
| **چالش‌های اخلاقی واقعی هستند**         | سوگیری، توهم‌زایی، محرمانگی ← نیازمند کنترل و راستی‌آزمایی    |
| **تفکر انتقادی ضروری است**              | هیچ خروجی مدل بدون بررسی نهایی قابل اعتماد نیست               |

AI را دستیار پژوهشی خود ببینید؛ قدرت تحلیل، خلاقیت و قضاوت علمی همچنان در دست شماست.

---

<!-- html -->
<div style="
  display: flex;
  gap: 30px;
  justify-content: center;
  align-items: center;
  height: 70vh;
">
  
  <div style="width: 25%; text-align: center;">
    <h2>پیوست</h2>
    <h3>
       فرصت‌های هوش مصنوعی در علوم/مهندسی کامپیوتر
    </h3>
    </div>
  <div style="width: 70%; text-align: center;">
    <video 
      autoplay 
      loop 
      muted 
      controls
      style="
        width: 100%;
        height: 60vh;
        border-radius: 10px;
        box-shadow: 0 5px 15px rgba(0,0,0,0.2);
      ">
      <source src="img/Classical-Academic-Researcher.mp4" type="video/mp4">
    </video>
  </div>
</div>

---

![bg opacity:0.22](img/cs-ai-opportunities-bg.jpg)

### ابزارهای هوش مصنوعی در علوم/مهندسی کامپیوتر

| حوزه                | کاربردهای کلیدی                                           | نمونه ابزارها                                                                                                                              |
| ------------------- | --------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ |
| **تسریع کدنویسی**   | تکمیل کد، دیباگ، بازنویسی تمیز، پیشنهاد معماری، Unit Test | [GitHub Copilot](https://github.com/features/copilot)، [Cursor](https://cursor.sh)، [Codex](https://platform.openai.com/docs/models/codex) |
| **تحلیل داده**      | تولید کد تحلیل، پیشنهاد روش آماری، نمودار و گزارش         | [ChatGPT](https://chatgpt.com)، [NotebookLM](https://notebooklm.google.com)، [Claude](https://claude.ai)                                       |
| **نمونه‌سازی سریع** | ساخت سریع MVP، front/back اولیه                           | [Lovable](https://lovable.dev)، [Qudo](https://qudo.ai)                                                                                    |
| **عامل (Agent)**   | بازسازی کل مخزن کد، اجرا و تست خودکار                | [Freebuff](https://freebuff.com)، [Copilot](https://github.com/features/copilot)                                                          |

---

![bg opacity:0.22](img/cs-ai-examples-bg.jpg)

## نمونه کاربردهای عملی AI در پروژه‌های کامپیوتری

- تولید نسخه اولیه (Prototype) از **backend** و **frontend** تنها با توصیف متنی
- تولید APIهای اولیه، مستندات، و تست‌های خودکار
<!-- - تبدیل ایده به شبه‌کد و به کد قابل‌اجرا -->
- ایجاد اسکریپت‌های کامل برای پیش‌پردازش داده
- پیشنهاد معماری مناسب برای مدل‌های یادگیری ماشین
- تولید گزارش تحلیلی از داده‌ها + توضیح نمودارها

> AI بهترین ابزار برای توسعه سریع نمونه اولیه در پروژه‌های دانشجویی و پژوهشی است.

---

![bg opacity:0.9](img/Curriculum_4_Disciplines.png)

## [جداول پیشنهادی دروس رشته‌های دانشکده علوم ریاضی ](https://mamintoosi-cs.github.io/tmp/ds/Curriculum_4_Disciplines.html) 

---

![bg opacity:0.8](img/copilot/20-RAG-start.png)

## سامانه پاسخگویی مبتنی بر RAG

در این پروژه، یک سامانه پاسخ‌گویی به پرسش مبتنی بر RAG طراحی و پیاده‌سازی شده است که به جای اتکا به دانش ضمنی مدل زبانی، ابتدا بخش‌های مرتبط از اسناد ورودی را بازیابی کرده و سپس پاسخ را فقط بر اساس همان شواهد تولید می‌کند.
کل سیستم، شامل بک‌اند، API و رابط کاربری وب، به‌صورت یکپارچه در محیط VSCode و با هوش مصنوعی مولد توسعه داده شده است.

---

![bg opacity:1](img/copilot/22-RAG-Results.png)

<!-- رابط کاربری امکان انتخاب مسیر اسناد، طرح پرسش، و مشاهده پاسخ به همراه شواهد و مراحل پردازش (retrieval، prompt و مدل) را فراهم می‌کند -->

---

![bg](img/copilot/20-RAG-copilot-commit.png)

 پیشنهاد خودکار متن کامیت

---

![bg opacity:1](img/my-vscode-screen-shot.png)

## VSCode

---

![bg](img/20th-century-enhanced.jpg)

<!-- # با تشکر از توجه شما 🙏

## پرسش و پاسخ -->

Thanks
_M. Amintoosi_
**.FUM, CS. Dept**

<!-- [mamintoosi.github.io](https://mamintoosi.github.io/)
[mamintoosi.github.io/presentations](https://mamintoosi.github.io/presentations/) -->
---