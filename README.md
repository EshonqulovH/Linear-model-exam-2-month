# Abalone Jismoniy Xususiyatlaridan Yoshni Bashorat Qilish

Ushbu loyihada abalonening turli jismoniy xususiyatlari asosida ularning yoshini bashorat qilish uchun bir nechta regressiya modellari qo'llanildi. Ma'lumotlar to'plamida abalone o'lchovlari mavjud bo'lib, yoshini (uzuklar soni orqali aniqlanadi) bashorat qilish maqsad qilingan.

## Mundarija
- [Loyiha Tavsifi](#loyiha-tavsifi)
- [Ma'lumotlar To'plami](#malumotlar-toplami)
- [O'rnatish](#ornatish)
- [Foydalanish](#foydalanish)
- [Modellashtirish Jarayoni](#modellashtirish-jarayoni)
  - [Xususiyatlarni Muhandislik](#xususiyatlarni-muhandislik)
  - [Regressiya Modellari](#regressiya-modellari)
  - [Ansambl Usullari](#ansambl-usullari)
  - [Stacking Regressor](#stacking-regressor)
- [Natijalar](#natijalar)
- [Xulosa](#xulosa)
- [Manbalar](#manbalar)

## Loyiha Tavsifi

Ushbu loyiha abalonening yoshini bashorat qilish uchun bir nechta mashinasozlik modellaridan foydalanadi. Ishlatilgan modellar quyidagilarni o'z ichiga oladi:
- Chiziqli Regressiya
- Ridge Regressiya
- Lasso Regressiya
- Huber Regressor
- RANSAC Regressor
- ElasticNet
- Polynomial Regressiya
- Stacking Regressor

Yakuniy model, Stacking Regressor, individual modellarning bashoratlarini birlashtirib, umumiy aniqlikni oshiradi.

## Ma'lumotlar To'plami

Ma'lumotlar to'plami abalonening o'lchovlaridan iborat bo'lib, quyidagilarni o'z ichiga oladi:
- Uzunlik
- Diametr
- Balandlik
- Og'irlik
- Tozalangan Og'irlik
- Ichki A'zolar Og'irligi
- Qobiq Og'irligi
- Jins (kategorik)

Ma'lumot to'plamining maqsadli o'zgaruvchisi - abalonening yoshi, bu uzuklar soni orqali aniqlanadi.

## O'rnatish

Kodlarni ishga tushirish uchun quyidagi kutubxonalarni o'rnatishingiz kerak:

```bash
pip install numpy pandas scikit-learn seaborn matplotlib
