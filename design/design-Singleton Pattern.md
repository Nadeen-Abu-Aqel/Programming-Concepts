<div align="right">

# 🔒 Singleton Pattern

## 📌 التعريف
Singleton هو Design Pattern يضمن أنه يوجد نسخة واحدة فقط من الكلاس في البرنامج.

## 💡 الفكرة الأساسية
بدل ما تنشئ أكثر من Object:
- يكون في Object واحد فقط  
- وكل الكود يستخدمه  

---

## 🔄 كيف يعمل؟
- تمنع إنشاء كائنات جديدة من الخارج  
- توفر Method ترجع نفس الـ Object دائمًا  

👉 يعني نفس النسخة تنستخدم بكل مكان

---

## 🔧 ماذا يوفر؟
توفير الذاكرة  
تنظيم الوصول للبيانات  
التحكم بكائن واحد  

---

## 🎯 متى نستخدمه؟
لما تحتاج Object واحد فقط مثل:
- Database Connection  
- Logger  
- Settings  

---

## ⚠️ ملاحظات
- الاستخدام الزائد ممكن يسبب مشاكل  
- يصعّب Testing أحيانًا  

---

## 🔥 مثال بسيط (Java)

```java
class Singleton {
    private static Singleton instance;

    private Singleton() {}

    public static Singleton getInstance() {
        if (instance == null) {
            instance = new Singleton();
        }
        return instance;
    }
}
```

---

## 📚 الخلاصة
Singleton = نسخة واحدة فقط من الكلاس  

👉 مفيد… بس لا تفرط باستخدامه 👍
