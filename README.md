# Mini Matrix — Providers (بدون سرور اصلی)

## ساختار
```
index.html
matrix_logo.png
providers/
  tradingview.js      # بدون کلید — پیش‌فرض
  goldapi_io.js       # نیاز به API Key
  unirateapi.js
  goldapi_net.js
  metals_api.js
  metalpriceapi.js
  tradermade.js
  api_ninjas.js
  goldprice_org.js
  goldprice_com.js
  mt5_local.js        # نیاز به سرور 127.0.0.1:8000 + EA
  index.js
```

## اجرا
فایل `index.html` را در مرورگر باز کنید (یا با Live Server در VS Code).
پوشه `providers` باید کنار `index.html` باشد.

## تست
از رادیو‌باتن‌ها یک منبع را انتخاب کنید.
اگر به API Key نیاز داشت، در کادر مربوطه وارد کنید (در localStorage ذخیره می‌شود).

## نکته CORS
بعضی APIها از مرورگر مستقیم بلاک می‌شوند. در آن صورت پیام خطا نشان داده می‌شود.
TradingView و (در صورت روشن بودن سرور) MT5 معمولاً بهترین گزینه‌های بدون دردسر هستند.
