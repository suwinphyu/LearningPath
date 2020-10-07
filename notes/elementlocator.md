## Selenium

ဒီတခါမှာတော့ Automation testing tool တစ်ခုဖြစ်တဲ့ 𝐒𝐞𝐥𝐞𝐧𝐢𝐮𝐦 (https://www.selenium.dev/downloads/) အကြောင်းလေ့လာကြရအောင်..
Selenium က web application အတွက်သာ အသုံးပြုလို့ရတဲ့ opensource testing tool တစ်ခုဖြစ်ပြီးတော့ မည်သည့် browser မှာမဆို အသုံးပြုလို့ရပါတယ်။ Test Script ရေးသားဖို့အတွက် အဓိက Language တွေအနေနဲ့ Ruby,Java,Python,C# and JavaScript တွေကို အသုံးပြုပြီးရေးသားနိုင်ပါတယ်။  တခြား PHP, Kotlin အစရှိသည်တို့ဖြင့်လည်း language binding လုပ်ပြီး အသုံးပြုနိုင်ပါတယ်။ 
အားနည်းချက်အနေနဲ့ကတော့ Configuration လုပ်ရာမှာ နည်းနည်းရှုပ်တယ်။ Images testing  လုပ်ဆောင်လို့မရနိုင်တဲ့အတွက် တခြား third-party tool(eg. Sikuli with selenium ) တွေနဲ့ integrate လုပ်ပေးရပါမယ်။ Built-in Reporting feature မပါတဲ့အတွက် Test report ထုတ်နိုင်ဖို့၊ Test Data တွေကို export ထုတ်နိုင်ဖို့အတွက် မိမိအသုံးပြုမယ့် language အလိုက် framework တွေ ထပ်ပေါင်းထည့်ပေးရပါမယ်( eg. Java အတွက်ဆို TestNG / JUnit) Test development လုပ်ဆောင်ရန်အတွက် သက်ဆိုင်ရာ Language အလိုက် coding အခြေခံ သဘောတရားကို နားလည်ထားရမှာဖြစ်တဲ့အတွက် ROI Time ကြာမြင့်နိုင်ပါတယ်။ Popup box handling အတွက် script ရေးသားရာမှာလည်း အမျိုးအစား (Alert / Pop up/confirmation / Prompt/ Authentication) နဲ့ testing environment တည်ဆောက်ထားသော OS (eg. Window/Linux) ပေါ်မူတည်ပြီး ပြောင်းလဲနိုင်ပါတယ်။
Selenium ရဲ့ components (၃) ခုကတော့
1. IDE (browser extension tool, records the users’ actions in the browser)
2. Grid (run test cases in  different machines across different platforms)
3. Web Driver (browser automation APIs)

#### IDE
IDE ကတော့ သုံးရတာလွယ်ကူတယ် Firefox and Chrome extension (eg.https://chrome.google.com/.../mooikfkahbdckldjjndioackbal... ) ပဲရှိတဲ့အတွက် တခြား browser တွေမှာ သုံးလို့မရပါဘူး ။ Setup လုပ်ထားသော URL ရဲ့ user action ကို record လုပ်ထားပေးပြီး test-case အနေနဲ့ generate လုပ်ယူနိုင်ပါတယ်။
#### Grid 
Grid ကိုတော့ Multiple Operation Systems (Nodes) ပေါ်မှာ browser အမျိုးမျိုးနဲ့ တပြိုက်နက်တည်း run တဲ့အခါမှာ အသုံးပြုနိုင်ပါတယ်။ Parallel Testing လုပ်နိုင်တဲ့အတွက် test execution time ကိုလျော့ချပေးနိုင်ပါတယ်။
#### Web Driver
Browser automation APIs တစ်ခုဖြစ်ပြီး ရေးသားထားသော test script များကို language အလိုက် interpret လုပ်ပေးပြီး browser ပေါ်တွင် automatically အလုပ်လုပ်နိုင်အောင် web-driver ကို အသုံးပြုခြင်းဖြစ်ပါတယ်။

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
