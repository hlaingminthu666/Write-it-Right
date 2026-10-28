# ✏️ Write It Right v2

ကျောင်းသား ကျောင်းသူများအတွက် **English Writing · Dictation · Picture Vocabulary** လေ့ကျင့်ခန်း App ပါ။ Notebook + red-pen ပုံစံ UI နဲ့ Internet မလိုဘဲ (Offline) သုံးနိုင်တဲ့ **PWA** ဖြစ်ပြီး ဖုန်း၊ Tablet၊ Computer အားလုံးမှာ ရပါတယ်။

## ✨ Features

**ရေးနည်းလေ့ကျင့်ခန်း (မူရင်း)**
- CSV / Excel (.xlsx) တင်ခြင်း၊ Excel row တွေကို paste လုပ်ခြင်း
- `( )` ပါလည်းရ မပါလည်းရ စကားလုံး၊ `||` အခြားအဖြေမှန်
- အဖြေမှားရင် ဆရာ့ red-pen နဲ့ ပြင်ပြပေးခြင်း၊ `Mode = self` ဆိုရင် ကိုယ်တိုင်စစ်ခြင်း
- စာလုံးအကြီးအသေး စစ်/မစစ်၊ Shuffle၊ Restart၊ Result၊ မှားတာတွေပဲ ထပ်လေ့ကျင့်ခြင်း
- အသံ effect၊ Mute၊ Full screen၊ **EN / မြန်မာ** UI

**🎧 Dictation (အသစ်)**
- Audio player: ▶ ဖွင့်/ရပ်၊ **🔁 Repeat (အစကနေ ပြန်ဖွင့်)**၊ ⟲ 5 စက္ကန့် နောက်ပြန်၊ အမြန်နှုန်း **0.75× / 1×**၊ ရှေ့/နောက် ဆွဲလို့ရတဲ့ bar
- `Start` / `End` နဲ့ အသံဖိုင်ရှည်တစ်ခုထဲက တစ်ပိုင်းချင်းကိုပဲ ဖွင့်နိုင်
- နားထောင်ခွင့် ကန့်သတ်ခြင်း (∞ / 1 / 2 / 3 / 5 ကြိမ်)
- စာရေးနေရင်း **Ctrl + Space** နှိပ်ပြီး ဖွင့်/ရပ်

**🖼 Picture Vocabulary (အသစ်)**
- ပုံကိုကြည့်ပြီး ဝေါဟာရ ရေးခြင်း
- **💡 Hint** ခလုတ်: နှိပ်တိုင်း စာလုံးတစ်လုံးစီ ပေါ်လာမယ် (`a p _ _ _`)
- ပုံကြီးတွေကို app က အလိုအလျောက် ချုံ့ပေးလို့ ဖုန်းမှာ မလေးဘူး

## 📤 File တင်နည်း

**Upload** ကိုနှိပ်ပြီး အောက်ပါနည်းနှစ်မျိုးထဲက တစ်မျိုးနဲ့ တင်ပါ:

1. **CSV/Excel နဲ့ အသံ၊ ပုံ file အားလုံးကို တစ်ခါတည်း ရွေးတင်** (Computer မှာ Ctrl / Shift နှိပ်ပြီး file အများကြီး ရွေးလို့ရ)
2. **ZIP တစ်ဖိုင်တည်း** တင်ခြင်း: CSV နဲ့ media file အားလုံးကို ZIP လုပ်ပြီး တင်ပါ (ဖုန်းမှာ အလွယ်ဆုံး)

- အသံ: `.mp3` (အကြံပြု), `.m4a`, `.wav`, `.ogg` …
- ပုံ: `.jpg`, `.png`, `.webp`, `.gif`, `.svg`
- File တွေကို **ဒီ device ထဲမှာပဲ** သိမ်းထားလို့ app ပိတ်ပြီး ပြန်ဖွင့်လည်း ကျန်နေမယ်။ ဖုန်းတစ်လုံးချင်းစီမှာ တစ်ခါ တင်ပေးရမယ်။
- CSV ထဲက file နာမည်နဲ့ တင်တဲ့ file နာမည် တူရမယ် (အကြီးအသေး မဆိုင်)။ မတွေ့တဲ့ file ရှိရင် app က နာမည်နဲ့တကွ ပြောပြပါမယ်။

## 📝 CSV Format

```csv
Instruction,Questions,Answer,Mode,Audio,Image,Start,End
Change into passive voice.,Mg Mg wrote a letter.,A letter was written by Mg Mg.,,,,,
Listen and write.,,I go to school by bus.,,lesson1.mp3,,,
,,She is reading a book.,,lesson2.mp3,,0:05,0:09
Look and write the word.,,elephant,,,elephant.jpg,,
,What is this?,an umbrella || umbrella,,,umbrella.png,,
```

| Column | အဓိပ္ပာယ် |
|---|---|
| Instruction | ညွှန်ကြားချက်။ အလွတ်ထားရင် အပေါ်ကဟာ ဆက်သုံး |
| Questions | မေးခွန်း။ Audio / Image ပါရင် အလွတ်ထားလို့ရ |
| Answer | အဖြေ (မဖြစ်မနေ)။ `( )` optional၊ `\|\|` အခြားအဖြေ |
| Mode | `self` = ကိုယ်တိုင်စစ်၊ အလွတ် = App က စစ် |
| Audio | အသံ file နာမည် (ဥပမာ `lesson1.mp3`) |
| Image | ပုံ file နာမည် (ဥပမာ `cat.jpg`) |
| Start / End | ဖွင့်မယ့်အပိုင်း: `0:05` (သို့) `5` စက္ကန့် (မထည့်လည်းရ) |

> မြန်မာစာ `????` ဖြစ်ရင် Excel မှာ **CSV UTF-8** နဲ့ save ပါ (သို့) `.xlsx` ကို တိုက်ရိုက်တင်ပါ။

## 🚀 GitHub Pages တင်နည်း / Update တင်နည်း

1. ZIP ကို **Extract** ဖြည်ပါ။
2. Repository ထဲမှာ **Add file → Upload files** → ZIP ထဲက file/folder အားလုံးကို ဆွဲထည့်ပါ (`icons` folder ပါ)။ ရှိပြီးသား file တွေကို အစားထိုးပါမယ်။ **Commit changes**။
3. ပထမဆုံးအကြိမ်ဆိုရင် **Settings → Pages** → `Deploy from a branch` → `main` / `(root)` → **Save**။
4. ၁–၂ မိနစ်အကြာ `https://<username>.github.io/<repo>/` မှာ ဖွင့်လို့ရပါပြီ။

> ⚠️ `index.html` က repository ရဲ့ root မှာ တိုက်ရိုက်ရှိရမယ်။
> ဒီ version မှာ `sw.js` ထဲက `VERSION = "wir-v2"` ဖြစ်ပြီးသား။ နောက်ထပ် update တင်ရင် `wir-v3` လို တိုးပေးပါ။

## 📲 Install လုပ်နည်း

- **Android (Chrome)**: ⋮ → **Install app / Add to Home screen**
- **iPhone / iPad (Safari)**: Share ⬆️ → **Add to Home Screen**
- **Computer (Chrome / Edge)**: Address bar ညာဘက်က Install icon

ပထမဆုံးတစ်ခါ **Internet ရှိချိန် ဖွင့်ပေးရမယ်**။ ပြီးရင် Offline ရပါပြီ။

## 🛠 ပြဿနာဖြေရှင်း

- **အသံမထွက်** → ဖုန်း silent mode ပိတ်ပါ၊ `.mp3` သုံးပါ၊ app ထဲက 🔇 Mute ကို စစ်ပါ
- **"File not found"** → Upload မှာ အဲဒီ file ကို ထပ်တင်ပါ (နာမည် spelling စစ်ပါ)
- **Update မပေါ်** → App ကို အပြီးပိတ်ပြီး ၂ ခါ ပြန်ဖွင့်ပါ
- **404** → Pages settings မှာ `main` + `/ (root)` စစ်ပါ

---
Made for Myanmar learners 🇲🇲
