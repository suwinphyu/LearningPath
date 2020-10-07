### Mocha
Mocha( https://mochajs.org/)ဆိုတာကတော့ unit testing အတွက်အသုံးပြုနိုင်တဲ့ JavaScript testing framework တစ်ခုပါ. asynchronous or synchronous code တွေအတွက်လည်း functionality test လုပ်ဆောင်နိုင်တယ်။ Mocha ကို any assertion library နဲ့တွဲသုံးနိုင်တယ်၊Chai assertion library နဲ့ တွဲသုံးတာများပါတယ်။ chai အကြောင်း အကြမ်းဖျင်း သိလိုပါက https://www.facebook.com/118132486588395/posts/136445608090416/?d=n တွင်လေ့လာနိုင်ပါတယ်။ 
Mocha ကို အသုံးပြုရန်အတွက် Node.js ဒါမှမဟုတ် browsers ပေါ်မှာ run နိုင်ပါတယ်. Node.js (https://nodejs.org/en/download/) ကိုအရင် install လုပ်ပါ။ npm (node package manager) ကို အသုံးပြုပြီးတော့ mocha(https://www.npmjs.com/package/mocha) ကို  𝘯𝘱𝘮 𝘪𝘯𝘴𝘵𝘢𝘭𝘭 𝘮𝘰𝘤𝘩𝘢 -𝘨 command နဲ့ globally install လုပ်ပေးရပါတယ်။ 

<img src="https://github.com/suwinphyu/readLists/blob/gh-pages/images/mocha1.jpg" width="650" height="300">

Project create လုပ်ရန်အတွက် project folder တစ်ခုဆောက်ပြီး. command line ကနေ 𝘯𝘱𝘮 𝘪𝘯𝘪𝘵 ကို project folder ထဲမှာ run ပေးလိုက်ရင် package.json file ကို generate လုပ်ပေးပါတယ်။ လိုအပ်တဲ့ configuration ကို package.json မှာ လုပ်ဆောင်လို့ရပါတယ်။ test folder တစ်ခုဆောက်ပြီး .js file မှာ mocha အတွက် test script တွေရေးသားနိုင်ပါတယ်။ Test script execute လုပ်ရန် command line မှ 𝘯𝘱𝘮 𝘵𝘦𝘴𝘵/𝘧𝘪𝘭𝘦𝘯𝘢𝘮𝘦.𝘫𝘴 ဟုခေါ် run နိုင်ပါတယ်။

<img src="https://github.com/suwinphyu/readLists/blob/gh-pages/images/mocha2.jpg" width="650" height="300">

Mocha မှာ describe() နဲ့ it() ဆိုတဲ့ pre-bundled function (၂) ခုရှိပါတယ်။ describe () function ကတော့ group of test case တနည်းအားဖြင့် test suits တစ်ခုပါပဲ။ describe () မှာ argument ၂ခုရှိပါတယ်။ တစ်ခုကတော့ name/description အတွက်ဖြစ်ပြီး နောက်တစ်ခုကတော့ call back function တစ်ခုပါ။
it() function ကတော့ individual test case တစ်ခုချင်းစီအတွက်သုံးနိုင်ပါတယ် describe() function အတွင်းထဲမှာ ရေးသားပေးရပါတယ်။ it() မှာလည်း argument 2 ခုရှိပါတယ်။ ပထမတစ်ခုကတော့ test case description နဲ့ နောက်တစ်ခုကတော့ test script function ဖြစ်ပါတယ်။
```
𝘥𝘦𝘴𝘤𝘳𝘪𝘣𝘦('𝘛𝘦𝘴𝘵 𝘚𝘶𝘪𝘵𝘦 - 𝘨𝘳𝘰𝘶𝘱 𝘰𝘧 𝘵𝘦𝘴𝘵 𝘤𝘢𝘴𝘦𝘴', 𝘧𝘶𝘯𝘤𝘵𝘪𝘰𝘯(){
𝘪𝘵('𝘵𝘦𝘴𝘵 𝘤𝘢𝘴𝘦 1', 𝘧𝘶𝘯𝘤𝘵𝘪𝘰𝘯(){ });
𝘪𝘵('𝘵𝘦𝘴𝘵 𝘤𝘢𝘴𝘦 2', 𝘧𝘶𝘯𝘤𝘵𝘪𝘰𝘯(){ });
𝘪𝘵('𝘵𝘦𝘴𝘵 𝘤𝘢𝘴𝘦 3', 𝘧𝘶𝘯𝘤𝘵𝘪𝘰𝘯(){ });
});
```

<img src="https://github.com/suwinphyu/readLists/blob/gh-pages/images/mocha3.jpg" width="650" height="300">

hook(https://mochajs.org/#hooks) ဆိုတာမျိုးက ဥပမာ အနေနဲ့ login process မလုပ်ခင် Captcha function ကို အလုပ်လုပ်ခိုင်းထားတဲ့ event တစ်ခုလိုမျိုးပါ။ mocha မှာ တော့ hook type (၄) မျိုး သုံးနိုင်ပါတယ်။
```
before() ကတော့ describe() ထဲမှာရှိတဲ့ test cases အားလုံး execute မလုပ်ခင်မှာ run ပါတယ်။

beforeEach() ကတော့ describe() ထဲမှာရှိတဲ့ test တစ်ခုချင်းစီ execute မလုပ်ခင်မှာ run ပါတယ်။

after() ကတော့ describe() ထဲမှာရှိတဲ့ test cases အားလုံး execute ပြီးတဲ့အခါမှ run ပါတယ်။

beforeEach() ကတော့ describe() ထဲမှာရှိတဲ့ test တစ်ခုချင်းစီ execute လုပ်ဆောင်ပြီးနောက် run ပါတယ်။
```

<img src="https://github.com/suwinphyu/readLists/blob/gh-pages/images/mocha4.jpg" width="650" height="300">

only(),skip() function တွေကတော့ အသုံးများတဲ့ Mocha test features တွေပါ။
only() ကိုတော့ only ကြေငြာထားတဲ့ test suite/test cases ကိုပဲ အလုပ်လုပ်ချင်တဲ့အခါမျိုးမှာ သုံးပြီးတော့ skip() ကတော့ pending test suite/test cases တွေအတွက် သုံးပါတယ်။

Resources : https://testautomationu.applitools.com/

