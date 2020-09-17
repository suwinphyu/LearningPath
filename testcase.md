Testing လုပ်ရမယ့် application အတွက် Test coverage (overall test plan) အရ မည့်သည့်အတိုင်းအတာထိ testing လုပ်ဆောင်ထားတယ်ဆိုတာကို အထောက်အထားနဲ့ ဖော်ပြနိုင်ဖို့ ၊ နောင်တချိန် retesting လုပ်တဲ့အခါမှာလည်း ပြန်လည်အသုံးပြုနိုင်အောင် အတွက် test case ကို ရေးသားကြတယ်
Don't Assume : Test Case ရေးသားရာတွင် application ၏ feature/functionality လုပ်ဆောင်ချက်တွေကို မိမိ ထင်မြင်ယူဆချက်အတိုင်း မရေးသားမိဖို့အရေးကြီးပါတယ်။ Software Requirement Specification (SRS) documents အတိုင်း အတိအကျ ရေးသားသင့်ပါတယ်။ အကယ်၍ requirement မပြည့်စုံပါက checklist တွေကို အကြံပြုနိုင်ပါတယ်။
Testcase ID, Test Description, Pre-condition, Steps to reproduce,Expected Result, Actual Result, Test Status, Test Data, Remarks,Test Executed by (Tester name),Test Execution Date စသည့် fields တွေကတော့ Test Case ရေးသားရာမှာ ယေဘုယျ ပါဝင်ကြတယ်

###### Pre-condition:
Testcase execution မလုပ်ခင်မှာ လိုအပ်တဲ့ requirement/ configurations အတွက်ပြင်ဆင်ထားရမည့်အချက်များ  ၊ တခြား test case ပြီးမှ လုပ်ဆောင်ရမည့် dependency case မျိုးဖြစ်နေလျှင် pre-executed test case id ကို  Pre-conditionတွင် ဖော်ပြနိုင်သည်။

###### Test Description:
Description ရေးသားရာတွင် မိမိ အဆင်ပြေသလို ပုံစံဖြင့် ရိုးရှင်းပြီး နားလည်လွယ်အောင် ရေးသားနိုင်သည်။ အောက်ပါ Basic Format of Test Case Description ပုံစံဖြင့်လည်း ဖော်ပြနိုင်သည်။ 
```
"Verify + What [dialog box, name] +When [condition] + How [action/place]"
```
###### Example:
1. Verify that user can send a friend request to any user by visiting their page
2. Verify that user can approve friend request from Notification
3. Verify that users receive a notification when these users get comments, Like or reactions on their posts

###### Steps to execute: 
Testing လုပ်ဆောင်ရမည့် step အဆင့်ဆင့်ကို နားလည်လွယ်ရန်အတွက် နံပါတ်စဉ်တပ်ပြီး ရေးသားထားခြင်းဖြစ်ပါတယ်။ Test case တစ်ခုမှာ Steps 3 ဆင့်ကနေ  Steps 8 ဆင့်အထိပဲ သတ်မှတ်ဖော်ပြသင့်ပါတယ် ။ Steps တွေအရမ်းများသွားရင် reproduce လုပ်ရာမှာ မလိုလားအပ်ပဲ ကြန့်ကြာမှုတွေဖြစ်နိုင်ပါတယ်။

###### Test Status:
Actual result နဲ့ expected result ကိုက်ညီမှုရှိလျှင် PASS လို့သတ်မှတ်နိုင်တယ်
Actual result နဲ့ expected result ကိုက်ညီမှုမရှိလျှင် Fail လို့သတ်မှတ်နိုင်တယ်
Testing လုပ်ရန် functionality အရအဆင်သင့်မဖြစ်သေးသော အခြေအနေတွင်  Not Available ၊   QA မစစ်ရသေးသော အခြေအနေကို Not Yet Tested စသည်ဖြင့် သတ်မှတ်နိုင်သည်။

Test case management tool တွေကို အသုံးပြုပြီး ရေးသားနိုင်ပါတယ်
https://www.guru99.com/top-20-test-management-tools.html - automatic!


Sample Test case format ကိုအောက်ပါ link တွင် လေ့လာနိုင်ပါတယ်
[Sample Test Case](https://github.com/suwinphyu/readLists/blob/gh-pages/Sample%20Test%20Case.xlsx)
