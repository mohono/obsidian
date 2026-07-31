# 📊 مثال‌های Dataview

> این فایل با پلاگین **Dataview** کار می‌کنه. کدها داخل بلاک‌های `dataview` هستن و خودشون رندر می‌شن.

## ۱. تسک‌های باز (از 10-Tasks)

```dataview
TASK FROM "10-Tasks"
WHERE !completed
```

## ۲. تسک‌های تکمیل‌شده

```dataview
TASK FROM "10-Tasks"
WHERE completed
```

## ۳. جدول یادداشت‌های روزانه (mood و weight از فرانت‌متر)

```dataview
TABLE mood, weight, date
FROM "20-Daily"
SORT date ASC
```

## ۴. یادداشت‌های تگ‌دار ورزش

```dataview
LIST FROM #ورزش
```

## ۵. تسک‌های سررسید‌دار امسال، گروه‌بندی بر اساس وضعیت

```dataview
TASK FROM "10-Tasks"
WHERE due
GROUP BY status
```
