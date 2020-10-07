### 𝗖𝗵𝗮𝗶
ဒီတခေါက်မှာတော့ 𝗖𝗵𝗮𝗶(https://www.chaijs.com/ ) ဆိုတဲ့ Assertion Library အကြောင်းဆွေးနွေးကြပါမယ်။  
assertion ဆိုတာ ဘယ်လိုမျိုးလဲ?ဘာကြောင့် သုံးရတာလဲ?
assert statement ဆိုတာ test တစ်ခုရဲ့ acceptance criteria နဲ့ကိုက်ညီတဲ့ expected result ကိုဖော်ပြတဲ့အခါမှာ သုံးနိုင်ပါတယ်။ Test တစ်ခုရဲ့ expected result နဲ့ actual result ကိုက်ညီလားဆိုတာကိုစစ်ဆေးနိုင်ဖို့အတွက် assertion library ကိုသုံးပြုနိုင်ပါတယ်။ Chai ကိုတော့ unit testing အတွက် Mocha နဲ့တွဲပြီး အသုံးများကြပါတယ်။
Chai ကို BDD (Behavior Driven Development) လို့ခေါ်တဲ့ readable language နဲ့ ရေးနိုင်သလို TDD(Test Driven Development) ပုံစံနဲ့လည်းရေးလို့ရပါတယ်။
BDD  style နဲ့ ရေးသားမယ်ဆိုရင်  𝗲𝘅𝗽𝗲𝗰𝘁 ဒါမှမဟုတ် 𝘀𝗵𝗼𝘂𝗹𝗱ကိုသုံးပါတယ်။ TDD style နဲ့ဆိုရင်တော့  𝗮𝘀𝘀𝗲𝗿𝘁ကိုသုံးပါတယ်။

#### 𝐞𝐱𝐩𝐞𝐜𝐭
ပထမဆုံး expect ( https://www.chaijs.com/guide/styles/#expect ) ကိုသုံးပြီး assertion ရေးကြည့်ရအောင်။ expect က BDD language ဖြစ်တာကြောင့် ဖတ်ရလွယ်တဲ့ keyword လေးတွေကို အသုံးပြုပြီး ရေးသားထားတဲ့ အတွက် မှတ်မိလွယ်ပါတယ်။ assertion ရေးသားရန်အတွက် chains ကို API reference (https://www.chaijs.com/api/bdd/ ) တွင်လေ့လာနိုင်ပါတယ်။
𝚟𝚊𝚛 𝚊𝚌𝚝𝚞𝚊𝚕_𝚊𝚗𝚜𝚠𝚎𝚛 = 𝟺𝟹;
𝚟𝚊𝚛 𝚎𝚡𝚙𝚎𝚌𝚝𝚎𝚍_𝚊𝚗𝚜𝚠𝚎𝚛 = 𝟺𝟹;
𝚎𝚡𝚙𝚎𝚌𝚝(𝚊𝚌𝚝𝚞𝚊𝚕_𝚊𝚗𝚜𝚠𝚎𝚛).𝚝𝚘.𝚎𝚚𝚞𝚊𝚕(𝚎𝚡𝚙𝚎𝚌𝚝𝚎𝚍_𝚊𝚗𝚜𝚠𝚎𝚛);

#### 𝐬𝐡𝐨𝐮𝐥𝐝
should (https://www.chaijs.com/guide/styles/#should) ကလည်း BDD style နဲ့ရေးသားနိုင်တဲ့အတွက် readable ဖြစ်တယ်. expect က modern browsers တွေအားလုံးကို support လုပ်ပေမယ့် should ကတော့ Internet Explorer ကလွဲပြီး တခြား browsers တွေကိုပဲ support လုပ်ပေးနိုင်ပါတယ်။ expect နဲ့ ကွာခြားတာကတော့ should က object တစ်ခုရဲ့ property အနေနဲ့ သုံးပါတယ်.
𝚟𝚊𝚛 𝚊𝚌𝚝𝚞𝚊𝚕_𝚊𝚗𝚜𝚠𝚎𝚛 = 𝟺𝟹;
𝚟𝚊𝚛 𝚎𝚡𝚙𝚎𝚌𝚝𝚎𝚍_𝚊𝚗𝚜𝚠𝚎𝚛 = 𝟺𝟹;
𝚊𝚌𝚝𝚞𝚊𝚕_𝚊𝚗𝚜𝚠𝚎𝚛.𝚜𝚑𝚘𝚞𝚕𝚍.𝚝𝚘.𝚎𝚚𝚞𝚊𝚕𝚜(𝚎𝚡𝚙𝚎𝚌𝚝𝚎𝚍_𝚊𝚗𝚜𝚠𝚎𝚛);

#### 𝐚𝐬𝐬𝐞𝐫𝐭
assert (https://www.chaijs.com/guide/styles/#assert ) ကတော့ TDD style နဲ့ ရေးသားထားတာဖြစ်ပြီး Node.js ရဲ့ default assert method တစ်ခုပဲဖြစ်ပါတယ်။ အရှေ့မှာ expect နဲ့ should ရေးသားထားပြီးတဲ့အတွက် assert သည်လည်း သဘောတရားချင်းအတူတူပါပဲ။
𝚟𝚊𝚛 𝚊𝚌𝚝𝚞𝚊𝚕_𝚊𝚗𝚜𝚠𝚎𝚛 = 𝟺𝟹;
𝚟𝚊𝚛 𝚎𝚡𝚙𝚎𝚌𝚝𝚎𝚍_𝚊𝚗𝚜𝚠𝚎𝚛 = 𝟺𝟹;
𝚊𝚜𝚜𝚎𝚛𝚝.𝚎𝚚𝚞𝚊𝚕(𝚊𝚌𝚝𝚞𝚊𝚕_𝚊𝚗𝚜𝚠𝚎𝚛,𝚎𝚡𝚙𝚎𝚌𝚝𝚎𝚍_𝚊𝚗𝚜𝚠𝚎𝚛);

Chai ကို အသုံးပြုဖို့အတွက် Node.js (https://nodejs.org/en/download/ ) ကိုအရင် install လုပ်ပေးရပါမယ်။ ပြီးရင် npm install chai -save-dev ဆိုပြီး chai ကို install လုပ်ဆောင်နိုင်ပါတယ်။ မိမိကြိုက်နှစ်သက်ရာ IDE ကို အသုံးပြုပြီး chai install လုပ်ထားတဲ့ project folder ထဲမှာ test folder တစ်ခုဆောက်ထားပြီး test script js file ကို ရေးပါ။



node test/filename.js ဆိုပြီး run လိုက်တဲ့အခါ assertion error မတက်ရင် PASS တယ်လို့သတ်မှတ်လို့ရပါတယ်။


expected result နဲ့ actual result မတူညီရင် assertion error ပြပါတယ်။ ဥပမာ မှာဆိုရင် expected result အနေနဲ့ object type ပါ ။ တကယ့် actual value က string type ဖြစ်နေတဲ့အတွက် assertion error ပြတယ်။


var expect = require('chai').expect;

var foo = 'bar';
expect(foo).to.be.a('string');
expect(foo).to.equal('bar');
expect(foo).to.have.lengthOf(3);

var beverages = {tea : ['chai','mocha','oolong','expresso']};
expect(beverages).to.have.property('tea').with.lengthOf(3);

var actual_answer = 43;
var expected_answer = 43;
expect(actual_answer).to.equal(expected_answer);
expect(actual_answer,"!!!Actual answer and expected one are different").to.equal(43); 

var should = require('chai').should();

var foo = 'bar';
foo.should.be.a('string');
foo.should.equal('bar');
foo.should.to.have.lengthOf(3);

var beverages = {tea : ['chai','mocha','oolong','expresso']};
beverages.should.to.have.property('tea').with.lengthOf(4);

var actual_answer = 43;
var expected_answer = 43;
actual_answer.should.to.equals(expected_answer);
actual_answer.should.to.equals(42,"!!!Actual answer and expected one are different"

var assert = require('chai').assert;

var foo = 'bar';
assert.typeOf(foo,'string');
assert.equal(foo,'bar');
assert.lengthOf(foo,3);

var beverages = {tea : ['chai','mocha','oolong','expresso']};
assert.property(beverages,'tea');
assert.lengthOf(beverages.tea,4);

var actual_answer = 43;
var expected_answer = 43;
assert.equal(actual_answer,expected_answer);
assert.equal(actual_answer,42,'!!!Actual answer and expected one are different');
