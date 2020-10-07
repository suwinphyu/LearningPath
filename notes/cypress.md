### Cypress
cypress (https://www.cypress.io/) ဆိုတာကတော့ JavaScript end-to-end open source tool တစ်ခုပါ။ front-end developer နဲ့ QA engineer တွေအတွက်ရည်ရွယ်ထားတဲ့ Testing tool လို့လည်းပြောလို့ရပါတယ်။ Chrome only ပဲအသုံးပြုလို့ရပါတယ်။ Selenium လိုမျိုး language အများကြီး support ပေးမထားပါဘူး။Only JavaScript ပဲရပါတယ်။ Test Runner အနေနဲ့ကတော့ Mocha (https://mochajs.org/) နဲ့တွဲသုံးရပါတယ်။ cypress ဆိုတာနဲ့ only JavaScript, only Chrome , only Mocha လို့ပြောလို့ရပါတယ်။ Cypress ရဲ့ အားသာချက်ကတော့ အရမ်းမြန်ဆန်ပြီး သုံးရတာလွယ်ကူတဲ့အတွက် နောက်ပိုင်း virtual testing အတွက် သုံးလာကြပါပြီ။ Fail task တွေအတွက် တခါတည်း screenshot ကိုထုတ်ပေးနိုင်တဲ့အပြင် Testing record အနေနဲ့ mp4 file လည်းထုတ်ပေးလိုက်သေးတယ်။

cypress ကိုသုံးဖို့အတွက် တခြား js framework တွေလိုမျိုး Node.js(https://nodejs.org/en/) install ထားရပါမယ်။ IDE ကတော့ ကြိုက်နှစ်သက်ရာသုံးနိုင်ပါတယ်။ ဒီမှာတော့ Visual Studio Code(https://code.visualstudio.com/) ကိုသုံးတာပါ။ ပထမဆုံး Project folder ဆောက်ပြီး terminal ကနေ 𝘯𝘱𝘮 𝘪𝘯𝘪𝘵 -𝘺 (𝘰𝘳) 𝘯𝘱𝘮 𝘪𝘯𝘪𝘵 သုံးပြီး package.json file ကို generate လုပ်ပေးတယ်။

ပြီးရင် npm install cypress ဆိုပြီး cypress ကို install လုပ်ပါ။

<img src="https://github.com/suwinphyu/readLists/blob/gh-pages/images/cypress1.png" width="650" height="300">


cypress install ပြီးတာနဲ့ 𝘯𝘱𝘹 𝘤𝘺𝘱𝘳𝘦𝘴𝘴 𝘰𝘱𝘦𝘯 ဆိုပြီး run ပေးရင် cypress.json file နဲ့ cypress folder ကိုမြင်တွေ့ရမှာပါ။

<img src="https://github.com/suwinphyu/readLists/blob/gh-pages/images/cypress2.png" width="650" height="300">


cypress folder ထဲက integration folder အောက်မှာ test.spec.js file တွေဆောက်ပြီး cypress ကိုစတင် အသုံးပြုနိုင်ပါပြီ။

<img src="https://github.com/suwinphyu/readLists/blob/gh-pages/images/cypress3.png" width="650" height="300">


Mocha မှာပါတဲ့ describe(), it() function တွေနဲ့ စတင် ပြီးtest script ရေးသားနိုင်ပါတယ်။ Mocha အကြောင်း အကြမ်းဖျဉ်းသိလိုပါက https://www.facebook.com/118132486588395/posts/136785401389770/?d=n တွင်လေ့လာနိုင်ပါတယ်။ cypress documentation(https://docs.cypress.io/api/api/table-of-contents.html) တွင်လည်း လေ့လာနိုင်ပါတယ်။

<img src="https://github.com/suwinphyu/readLists/blob/gh-pages/images/cypress4.png" width="650" height="300">


element locator ကို inspect icon လေးနဲ့ ထောက်ပြီး အလွယ်တကူ copy ကူးယူသုံးနိုင်တဲ့အတွက် web element locator အတွက် အချိန်ပေးစရာမလိုတော့ပါဘူး။

<img src="https://github.com/suwinphyu/readLists/blob/gh-pages/images/cypress5.png" width="650" height="300">


assertion အတွက် Chai assertion (https://docs.cypress.io/guides/references/assertions.html...) ကိုသုံးလို့ရပါတယ်။
<img src="https://github.com/suwinphyu/readLists/blob/gh-pages/images/cypress6.png" width="650" height="300">


ဒါကတော့ cypress run တဲ့အခါ ပြပေးတဲ့ automated browser ပါ။ဘေးမှာတော့ Tasks list and result တွေဖော်ပြထားပါတယ်။
<img src="https://github.com/suwinphyu/readLists/blob/gh-pages/images/cypress7.png" width="650" height="300">


mocha ရဲ့hook တွေဖြစ်တဲ့ before, beforeEach, after, afterEach တွေကို သုံးနိုင်သလို only(), skip() function တွေနဲ့လည်း cypress ကို run လို့ရပါတယ်။
<img src="https://github.com/suwinphyu/readLists/blob/gh-pages/images/cypress8.png" width="650" height="300">


ဥပမာမှာဆိုရင် URL ကိုခေါ်တဲ့ test ကို before hook နဲ့ရေးထားတဲ့အတွက် test case တွေအားလုံး မစခင် before function ကအရင်အလုပ်လုပ်ပါမယ် ။ ပြီးရင်တော့ Only() လို့သတ်မှတ်ထားတဲ့ test case ကိုပဲ run မှာဖြစ်ပါတယ်။
<img src="https://github.com/suwinphyu/readLists/blob/gh-pages/images/cypress9.png" width="650" height="300">

<img src="https://github.com/suwinphyu/readLists/blob/gh-pages/images/cypress10.png" width="650" height="300">

Resources : https://testautomationu.applitools.com/
