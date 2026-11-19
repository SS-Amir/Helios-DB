<div dir="rtl">

**🇬🇧 [English](README.md) | 🇮🇷 فارسی**

# پروژه پایگاه داده - سیستم مدیریت پنل خورشیدی

**گروه:** نیما اشراقی، علی پاشایی، امیرحسین صانعیان

## مراحل پروژه
- [x] مرحله ۱ — سند نیازمندی‌ها
- [x] مرحله ۲ — مدل ER
- [ ] مرحله ۳ — طرح رابطه‌ای
- [ ] مرحله ۴ — نرمال‌سازی
- [ ] مرحله ۵ — پیاده‌سازی SQL
- [ ] مرحله ۶ — آزمون و کوئری‌ها

## مستندات مراحل
### مرحله ۱ — نیازمندی‌ها
| قالب | 🇬🇧 انگلیسی | 🇮🇷 فارسی |
|:--|:--|:--|
| 📝 Markdown | [`01-requirements.md`](docs/01-requirements.md) | [`01-requirements.fa.md`](docs/01-requirements.fa.md) |
| 📄 PDF | [`Helios-db-RC.pdf`](docs/source/Helios-db-RC.pdf) | [`Helios-db-RC-fa.pdf`](docs/source/Helios-db-RC-fa.pdf) |
| 📦 Source (`.docx`) | [`Helios-db-RC.docx`](docs/source/Helios-db-RC.docx) | [`Helios-db-RC-fa.docx`](docs/source/Helios-db-RC-fa.docx) |

### مرحله ۲ — مدل ER

| قالب | 🇬🇧 انگلیسی | 🇮🇷 فارسی |
|:--|:--|:--|
| 📝 Markdown | [`02-er-diagram.md`](docs/02-er-diagram.md) | [`02-er-diagram.fa.md`](docs/02-er-diagram.fa.md) |
| 🎨 منبع نمودار (`.drawio`) | [`Helios-db-ER.drawio`](diagrams/Helios-db-ER.drawio) | [`Helios-db-ER-fa.drawio`](diagrams/Helios-db-ER-fa.drawio) |
| 🖼️ نمودار (SVG) | [`Helios-db-ER.drawio.svg`](diagrams/Helios-db-ER.drawio.svg) | [`Helios-db-ER-fa.drawio.svg`](diagrams/Helios-db-ER-fa.drawio.svg) |

## ساختار پروژه
</div>

<div dir="ltr">

```
Helios-DB/
├── README.md
├── README.fa.md
├── .gitignore
├── .gitattributes
├── docs/
│   ├── requirements.md
│   ├── requirements.fa.md
│   ├── 02-er-diagram.md
│   ├── 02-er-diagram.fa.md
│   └── source/
│       ├── Helios-db-RC.docx
│       ├── Helios-db-RC.pdf
│       ├── Helios-db-RC-fa.docx
│       └── Helios-db-RC-fa.pdf
├── diagrams/
│   ├── Helios-db-ER.drawio
│   ├── Helios-db-ER.drawio.svg
│   ├── Helios-db-ER-fa.drawio
│   └── Helios-db-ER-fa.drawio.svg
└── sql/
    └── queries/
```

</div>

<div dir="rtl">

## نحوه اجرای SQL
_تکمیل می‌شود._

## یادداشت‌ها
- فایل‌های PDF در `docs/source/` از فایل‌های `.docx` تولید می‌شوند. در صورت تغییر `.docx`، دوباره تولید شوند.
- اگر نمایشگر PDF در GitHub با خطا مواجه شد، از دکمه **Download** استفاده کنید یا `?raw=true` را به انتهای آدرس PDF اضافه کنید تا در نمایشگر داخلی مرورگر باز شود.
- **اصلاحیه:** فایل‌های PDF در `docs/source/` در کامیت 3158c5cdfdc9ae56bcd86521c268131793e77a83 اصلاح شدند. تگ `v0.1-requirements` نسخهٔ پیش از اصلاح را دارد.
---

> این README به زبان [انگلیسی](README.md) نیز موجود است. هر تغییری در وضعیت پروژه، ساختار یا فهرست مراحل در **هر دو** فایل اعمال می‌شود.

---

## برچسب‌ها (Tags)

هر مرحله با یک برچسب annotated علامت‌گذاری می‌شود تا بتوانید به یک مرحلهٔ تمام‌شده برگردید یا تفاوت دو مرحله را ببینید.

| برچسب | مرحله | وضعیت |
|---|---|---|
| `v0.1-requirements` | مرحله ۱ — نیازمندی‌ها | ✅ انجام شد |
| `v0.2-er-model` | مرحله ۲ — مدل ER | ✅ انجام شد |
| `v0.3-relational-schema` | مرحله ۳ — طرح رابطه‌ای | ⏳ برنامه‌ریزی‌شده |
| `v0.4-normalization` | مرحله ۴ — نرمال‌سازی | ⏳ برنامه‌ریزی‌شده |
| `v0.5-sql` | مرحله ۵ — پیاده‌سازی SQL | ⏳ برنامه‌ریزی‌شده |
| `v1.0-final` | مرحله ۶ — آزمون و تحویل نهایی | ⏳ برنامه‌ریزی‌شده |

**کامندهای کاربردی**
```bash
git tag -n                                   # فهرست برچسب‌ها همراه پیام
git checkout v0.1-requirements               # دیدن یک مرحلهٔ تمام‌شده (detached HEAD)
git switch -                                 # بازگشت به جای قبلی
git diff v0.1-requirements..v0.2-er-model    # تفاوت دو مرحله
```
</div>
