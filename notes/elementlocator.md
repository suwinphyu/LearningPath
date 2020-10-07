### Element Locator for Test Automation

Element locator ကိုလေ့လာဖို့အတွက် HTML,CSS,JavaScript ကို အခြေခံသိရှိထားရပါမယ်။ Manually အနေနဲ့ web page တစ်ခုကို scroll ဆွဲတာ၊  button click လိုက်တာ၊ keyword တစ်ခုခုရိုက်ထည့်ပြီး search လုပ်တာမျိုးက လွယ်ကူပေမယ့် Test Automation အတွက် DOM (Document Object Model) တွေကို တိတိကျကျရှာဖွေနိုင်ဖို့အတွက် locator တွေနဲ့ ညွှန်းဖို့လိုအပ်ပါတယ်။
အောက်ဖော်ပြပါ Locator types  တွေထဲက တစ်နည်းနည်းကို အသုံးပြုပြီး ရေးသားနိုင်ပါတယ်။ 
1. ID (if unique on the page)
2. Name (if unique on the page)
3. Class name
4. CSS Selector
5. XPath
6. Link Text and Partial Link Text
7. TagName
နမူနာ အနေနဲ့ Chrome dev tool (https://developers.google.com/web/tools/chrome-devtools/) ကို အသုံးပြုပြီးတော့ https://duckduckgo.com/ အတွက် Locator ရှာကြည့်ရအောင်။ အသေးစိတ်ကိုတော့ screenshots လေးတွေမှာ လေ့လာကြည့်ပေးကြပါနော်။




#### ID
Search box အတွက် test script ရေးသားဖို့ ID ကိုအသုံးပြုနိုင်တယ်။ အလွယ်ဆုံးနည်းလမ်းဖြစ်ပြီး unique လည်းဖြစ်တယ်
<img src="https://github.com/suwinphyu/readLists/blob/gh-pages/images/locator1.png" width="680" height="300">

#### Name
တကယ်လို့ Element မှာ ID မပါဘူးဆိုရင် Name ကိုရှာကြည့်ပါ။ Name attribute သည်လည်း Unique ဖြစ်တဲ့အတွက် အသုံးပြုရလွယ်ကူတယ်
<img src="https://github.com/suwinphyu/readLists/blob/gh-pages/images/locator2.png" width="680" height="300">

#### Class Name
Classname ရှာရာတွင် class တစ်ခုကို multiple elements တွေ ခေါ်သုံးတာမျိုးရှိတတ်သဖြင့် သေချာစီစစ်ပြီးမှ သုံးသင့်ပါတယ်။
<img src="https://github.com/suwinphyu/readLists/blob/gh-pages/images/locator3.png" width="680" height="300">

#### CSS Selector
Chrome Dev tool ကိုအသုံးပြုပြီး copy selector လုပ်နိုင်ပါတယ်။
<img src="https://github.com/suwinphyu/readLists/blob/gh-pages/images/locator4.png" width="680" height="300">

#### XPath
Chrome Dev tool ကိုအသုံးပြုပြီး copy xpath လုပ်နိုင်ပါတယ်။
<img src="https://github.com/suwinphyu/readLists/blob/gh-pages/images/locator5.png" width="680" height="300">

#### Link Text and Partial Link Text
Partial Link Text ကို နောက်screenshot တွင်ဖော်ပြထားပါတယ်
<img src="https://github.com/suwinphyu/readLists/blob/gh-pages/images/locator6.png" width="680" height="300">
                                                                                                           
#### Tag Name
<img src="https://github.com/suwinphyu/readLists/blob/gh-pages/images/locator7.png" width="680" height="300">

Resources : https://testautomationu.applitools.com/
