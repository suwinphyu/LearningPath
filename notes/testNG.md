
TestNG installation step by step ကို ဖော်ပြပါ link အတိုင်း လုပ်ဆောင်နိုင်ပါတယ်။
https://intellipaat.com/blog/tutorial/selenium-tutorial/testng-in-selenium/
https://www.toolsqa.com/testng/install-testng/

Chrome WebDriver အတွက် https://chromedriver.chromium.org/downloads

#### TestNG new repository link
Name: TestNG (depends on the user), Location: https://dl.bintray.com/testng-team/testng-eclipse-release/6.14.3/

Test case တွေမှာ pre-conditions ၊ post-conditions တွေထည့်ရေးရတာမျိုးရှိသလို TestNG မှာလည်း Annotation သုံးပြီး pre-conditions ဆိုရင် @Before ၊ post-conditions ဆိုရင် @After နဲ့အစပြုပြီးရေးနိုင်ပါတယ်။ Test Steps တွေအတွက်တော့ @Test နဲ့ရေးသားနိုင်ပါတယ်။

<img src="https://github.com/suwinphyu/readLists/blob/gh-pages/images/annotation.jpg" width="680" height="300">

TestNG ရဲ့ default execution order အနေနဲ့က alphabetical order (A – Z) အလိုက် @Test run တဲ့အတွက် SearchCustomer နဲ့ Login Test ဆိုရင် Login function ကအရင် run တယ်။

<img src="https://github.com/suwinphyu/readLists/blob/gh-pages/images/alphabetical.jpg" width="680" height="300">

priority attribute ကို @Test မှာသုံးပြီးတော့ test execution order ကိုသတ်မှတ်ပေးလို့ရတယ်။ @Test (priority= Integer data type) lowest number ကအရင်ဆုံး execute လုပ်ပေးတယ်

<img src="https://github.com/suwinphyu/readLists/blob/gh-pages/images/priority.jpg" width="680" height="300">

Assertion functions (assertTrue ,assertFalse ,assertSame ,assertNotSame ,assertNotNull ,assertEquals )ကိုသုံးပြီး expected result နဲ့ Output result မှန်မမှန်စစ်ဆေးနိုင်တယ်

<img src="https://github.com/suwinphyu/readLists/blob/gh-pages/images/assertion.jpg" width="680" height="300">

TestNG ရဲ့ အားသာချက်ထဲက တစ်ခုကတော့ Dependency feature ပါပဲ. Method တစ်ခုဟာ တခြား methods တွေပေါ်မှာ မှီခိုပြီးမှ execute လုပ်နိုင်တဲ့အခြေအနေမျိုးမှာ dependsOn attribute ကိုသုံးနိုင်ပါတယ်။ ဥပမာအနေနဲ့ signout method ဟာ signin ပြီးမှကို အလုပ်လုပ်လို့ရနိုင်တာမျိုးပါ။ Signout အလုပ်လုပ်ဖို့က signin method ပေါ်မှာ depend ဖြစ်နေတာမျိုးပါ။

<img src="https://github.com/suwinphyu/readLists/blob/gh-pages/images/dependsonMethod.jpg" width="680" height="300">

Development , QA , Staging , Production စတဲ့ testing environment တွေရဲ့ URL တွေကမတူညီကြတဲ့အခါမျိုးမှာ @Test တွေကို group အလိုက်ခွဲပြီးသတ်မှတ်လို့ရတယ်။  XML file ထဲမှာ execute လုပ်ချင်တဲ့  group name ကို include ကြေငြာပေးပြီး xml file ကို run လိုက်တာတဲ့ only include group ပဲ အလုပ်လုပ်သွားတယ်။ exclude ကိုသုံးပြီးလည်း exclude group ကလွဲလို့ကျန်တဲ့ group တွေ အကုန် အလုပ်လုပ်မယ်ဆိုပြီးလည်း ကြေငြာလို့ရတယ်။ dependonMethod လိုပဲ dependonGroup နဲ့လည်း group တစ်ခုခုပေါ်မှာ depend ဖြစ်တဲ့အခါအသုံးပြုနိုင်တယ်။ 

<img src="https://github.com/suwinphyu/readLists/blob/gh-pages/images/group.jpg" width="680" height="300">

Data Driver testing အတွက်Java objects တွေကို  @DataProvider အနေနဲ့ data passing လုပ်ပေးပြီးအသုံးပြုနိုင်တယ်

<img src="https://github.com/suwinphyu/readLists/blob/gh-pages/images/dataprovider.jpg" width="680" height="300">

Project ကို refresh လုပ်ပြီး test-output folder ထဲမှာ emailable-report.html ကနေ test result ကြည့်နိုင်ပါတယ်။

<img src="https://github.com/suwinphyu/readLists/blob/gh-pages/images/Output.jpg" width="680" height="300">



Reference Source:
https://intellipaat.com/
https://www.toolsqa.com/
https://applitools.com/
