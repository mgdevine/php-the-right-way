---
isChild: true
anchor:  mac_setup
---

## Mac Setup {#mac_setup_title}

OS X မှာ PHP ကို prepackaged လုပ်ပြီးသားရှိပါတယ် ဒါပေမယ့်ပုံမှန်အားဖြင့်အဲ့ဒါက နောက်ဆုံး version ထက်နောက်ကျနေပါတယ်။ Mountain Lion မှာ 5.3.10၊ Mavericks မှာ 5.4.17 နဲ့ Yosemite မှာ 5.5.9 ရှိပါတယ်၊ ဒါပေမယ့် PHP 5.6 ထွက်လာတဲ့အခါမှာဒါတွေကမလုံလောက်တော့ပါဘူး။

PHP ကို OS X မှာ install လုပ်ဖို့နည်းမျိူးစုံရှိပါတယ်

### Homebrew ကနေ PHP ကို Install လုပ်ခြင်း

[Homebrew] က OS X အတွက် powerful package manager တစ်ခုဖြစ်ပါတယ်၊ သူက PHP နဲ့ အခြား extensions တွေကို install လုပ်ဖို့ သင့်ကိုကူညီနိုင်ပါတယ်။
[Homebrew PHP] ကတော့ repository တစ်ခုဖြစ်ပါတယ် အဲ့ဒါက Homebrew အတွက် PHP နဲ့ပတ်သတ်တဲ့ "formulae" တွေပါဝင်ပါတယ်၊ နောက်ပြီး အဲ့ဒါကသင့်ကို PHP install လုပ်ခွင့်ပြုပါလိမ့်မယ်။

ဒီနေရာမှာတော့၊ သင် `php53`, `php54`, `php55` ဒါမှမဟုတ် `php56` တွေကို `brew install` command နဲ့ install လုပ်နိုင်ပါတယ်၊ နောက်အဲ့ဒါတွေကိုလည်း သင် modify လုပ်ထားတဲ့ `PATH` variable ပေါ်မူတည်ပြီးတော့လည်းပြောင်းလဲနိုင်ပါတယ်။ 

### PHP ကို phpbrew ကနေတစ်ဆင့် Install လုပ်ခြင်း

[phpbrew] က PHP install လုပ်ဖို့ tool တစ်ခုလည်းဖြစ်တယ် နောက် PHP versions တွေကိုလည်း managing လုပ်ပေးပါတယ်။ ဒါက မတူညီတဲ့ applications/projects နှစ်ခုက မတူညီတဲ့ PHP version နှစ်ခုလိုတယ် နောက် သင်က virtual machines လည်းမသုံးဘူးဆိုရင်ဒါကတကယ့်ကိုအသုံးဝင်မှာဖြစ်ပါတယ်။

### Compile from Source

နော်ထက်ရွေးချယ်စရာတစ်ခုကတော့ ကိုယ်တိုင် compile လုပ်တာပါဘဲ[compile it yourself][mac-compile]၊ compile လုပ်မယ်ဆိုရင် [Xcode][xcode-gcc-substitution] ဒါမှမဟုတ် Apple's substitute
["Command Line Tools for XCode"] ကို Apple's Mac Developer Center ကနေ download လုပ်ပြီး install လုပ်ထားရပါမယ်။

### All-in-One Installers

The solutions listed above mainly handle PHP itself, and do not supply things like Apache, Nginx or a SQL server.
"All-in-one" solutions such as [MAMP][mamp-downloads] and [XAMPP][xampp] will install these other bits of software for
you and tie them all together, but ease of setup comes with a trade-off of flexibility.

အထက်မှာဖော်ပြခဲ့တဲ့ solution တွေကတော့ PHP အတွက်ဘဲဖြေရှင်းသွားတာတွေဖြစ်ပါတယ်၊Apache, Nginx လို Webserver တွေ SQL server တွေကိုတော့ support ပေးမှာမဟုတ်ပါဘူး။ "All-in-one" ဆိုတာကတော့ [MAMP][mamp-downloads] and [XAMPP][xampp]


[Homebrew]: http://brew.sh/
[Homebrew PHP]: https://github.com/Homebrew/homebrew-php#installation
[phpbrew]: https://github.com/phpbrew/phpbrew
[mac-compile]: http://php.net/install.macosx.compile
[xcode-gcc-substitution]: https://github.com/kennethreitz/osx-gcc-installer
["Command Line Tools for XCode"]: https://developer.apple.com/downloads
[mamp-downloads]: http://www.mamp.info/en/downloads/
[xampp]: http://www.apachefriends.org/en/xampp.html
