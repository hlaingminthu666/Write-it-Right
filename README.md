# ✏️ Write It Right

ကျောင်းသား ကျောင်းသူများအတွက် **English Writing Practice** App ဖြစ်ပါတယ်။ Notebook + red-pen ပုံစံ UI နဲ့ Internet မရှိဘဲ (Offline) လေ့ကျင့်နိုင်တဲ့ **PWA** ဖြစ်ပြီး ဖုန်း၊ Tablet၊ Computer အားလုံးမှာ သုံးနိုင်ပါတယ်။

## ✨ Features

- CSV / Excel (.xlsx) ဖိုင်တင်ပြီး လေ့ကျင့်ခန်းဖန်တီးခြင်း၊ Excel row တွေ paste လုပ်ခြင်း
- `( )` = ပါလည်းရ မပါလည်းရ စကားလုံး၊ `||` = အခြားမှန်တဲ့အဖြေ
- `Mode = self` ဆိုရင် ကျောင်းသားကိုယ်တိုင် နမူနာအဖြေနဲ့ တိုက်စစ်
- စာလုံးအကြီးအသေး စစ်/မစစ် ရွေးနိုင်
- Shuffle၊ Restart၊ Result screen၊ မှားတာတွေပဲ **Try Again**
- အသံ effect နဲ့ Mute၊ Full screen
- **EN / MM** UI ဘာသာစကား ပြောင်းနိုင် (English default)
- တင်ထားတဲ့ လေ့ကျင့်ခန်းကို browser မှာ မှတ်ထား
- Home screen ထဲ App အဖြစ် Install လုပ်ပြီး Offline သုံးနိုင်

## 📁 Files

```
index.html             ← App (မူရင်း UI အတိုင်း)
manifest.webmanifest   ← PWA အချက်အလက်
sw.js                  ← Offline cache
icons/                 ← App icon (192, 512, Apple, SVG)
.nojekyll
README.md
```

## 🚀 GitHub Pages တင်နည်း

1. ZIP ကို **Extract** ဖြည်ပါ။
2. GitHub မှာ Repository အသစ် ဖန်တီးပါ (ဥပမာ `write-it-right`)၊ **Public** ထားပါ။
3. **Add file → Upload files** နှိပ်ပြီး ZIP ထဲက file/folder အားလုံးကို ဆွဲထည့်ပါ (`icons` folder ပါ ပါရမယ်)။ **Commit changes** နှိပ်ပါ။
4. **Settings → Pages** သွားပါ။
5. **Source** = `Deploy from a branch`၊ **Branch** = `main`၊ folder = `/ (root)` ရွေးပြီး **Save**။
6. ၁–၂ မိနစ်စောင့်ပါ။ Link ရပါမယ်: `https://<username>.github.io/write-it-right/`

> ⚠️ `index.html` က Repository ရဲ့ root မှာ တိုက်ရိုက်ရှိရပါမယ်။ folder တစ်ဆင့်အောက်ရောက်နေရင် 404 ပြပါမယ်။
> `.nojekyll` က hidden file ဖြစ်လို့ မမြင်ရရင် မတင်လည်း App အလုပ်လုပ်ပါတယ်။

## 📲 Install လုပ်နည်း

- **Android (Chrome)**: Link ဖွင့် → ⋮ menu → **Install app / Add to Home screen**
- **iPhone / iPad (Safari)**: Share ⬆️ → **Add to Home Screen**
- **Computer (Chrome / Edge)**: Address bar ညာဘက်က Install ⊕ icon

ပထမဆုံးတစ်ခါ **Internet ရှိချိန်မှာ ဖွင့်ပေးရပါမယ်**။ ပြီးရင် Offline မှာ ဖွင့်လို့ရပါပြီ။

## 📝 CSV Format

```csv
Instruction,Questions,Answer,Mode
Change into passive voice.,Mg Mg wrote a letter.,A letter was written by Mg Mg.,
,They are building a new school.,A new school is being built (by them).,
Answer the question.,What did you do yesterday?,I went to the market.,self
```

| Column | အဓိပ္ပာယ် |
|---|---|
| Instruction | ညွှန်ကြားချက်။ အလွတ်ထားရင် အပေါ်ကဟာ ဆက်သုံး |
| Questions | မေးခွန်း (မဖြစ်မနေ) |
| Answer | အဖြေ (မဖြစ်မနေ)။ `( )` optional၊ `\|\|` အခြားအဖြေ |
| Mode | `self` = ကိုယ်တိုင်စစ်၊ အလွတ် = App က စစ် |

> မြန်မာစာ `????` ဖြစ်နေရင် Excel မှာ **CSV UTF-8** နဲ့ save ပါ (သို့) `.xlsx` ကို တိုက်ရိုက်တင်ပါ။

## 🔄 Update တင်နည်း

`index.html` ပြင်ပြီး ပြန်တင်တိုင်း `sw.js` ထဲက `VERSION` ကို တိုးပေးပါ:

```js
const VERSION = "wir-v1";   →   const VERSION = "wir-v2";
```

မတိုးရင် ကျောင်းသားတွေ ဖုန်းမှာ version အဟောင်းပဲ ဆက်ပြနေနိုင်ပါတယ်။

## 🛠 ပြဿနာဖြေရှင်း

- **404** → Pages settings မှာ `main` + `/ (root)` ဟုတ်မဟုတ် စစ်ပါ
- **Install ခလုတ် မပေါ်** → `https://` link ဖြစ်ရမယ်၊ `icons` folder ပါမပါ စစ်ပါ
- **Update မပေါ်** → `VERSION` တိုးပြီး App ကို ပိတ်ပြီး ၂ ခါ ပြန်ဖွင့်ပါ
- **Font ပုံစံ ပြောင်းနေ** → Internet နဲ့ တစ်ခါဖွင့်ပေးရင် font တွေ cache ဖြစ်သွားပါမယ်

---
Made for Myanmar learners 🇲🇲
