# minibrooo
**Проект в разработке**  
«MiniBro» – это мобильное приложение, позволяющее пользователям заказывать доставку еды, товаров и посылок с помощью автономных роботов-курьеров. Это не просто доставка, а удобный, безопасный и технологичный сервис, который решает проблемы традиционных курьерских служб

Функционал:
- [x] Просмотр доступных роботов на карте
- [x] Оформление заказа
- [ ] Отслеживание текущего заказа
- [x] История заказов
- [x] Оценка доставки и оставление отзыва
- [ ] Профиль пользователя и платёжные данные
- [ ] Push-уведомления о статусе заказа

Используемые технологии:
- **Язык:** Kotlin
- **UI:** Jetpack Compose
- **Навигация:** Jetpack Navigation
- **Карта:** Google Maps SDK
- **База данных и авторизация:** Firebase (Firestore, Auth)
- **Архитектура:** MVVM (ViewModel, LiveData)
- **Асинхронность:** Kotlin Coroutines
- **Сборка:** Gradle
  
Запуск проекта

1. **Склонируйте репозиторий**:
   ```bash
   git clone https://github.com/Nanivooo/minibrooo.git
2. **Откройте проект в Android Studio**
3. **Добавьте файл google-services.json:**
Скачайте его из Firebase Console и поместите в папку:
app/google-services.json
4. **Укажи API-ключ Google Maps**  
   Вставь его в `AndroidManifest.xml`:  
   ```xml
   <meta-data android:name="com.google.android.geo.API_KEY" android:value="ВАШ_КЛЮЧ" />
5. **Синхронизируйте Gradle:**
Нажмите "Sync Project with Gradle Files" в Android Studio
6. **Запустите проект:**
Используйте эмулятор или физическое устройство (Android 8.0+)

Зависимости (`build.gradle`)
<details>
<summary>Нажми, чтобы раскрыть зависимости</summary>

```kotlin
// Firebase
implementation(platform("com.google.firebase:firebase-bom:32.3.1"))
implementation("com.google.firebase:firebase-auth-ktx")
implementation("com.google.firebase:firebase-firestore-ktx")

// Compose
implementation("androidx.compose.ui:ui")
implementation("androidx.navigation:navigation-compose")
implementation("androidx.lifecycle:lifecycle-viewmodel-compose")

// Coil
implementation("io.coil-kt:coil-compose:2.4.0")

// Retrofit
implementation("com.squareup.retrofit2:retrofit:2.9.0")
implementation("com.squareup.retrofit2:converter-gson:2.9.0")

// Kotlin coroutines
implementation("org.jetbrains.kotlinx:kotlinx-coroutines-android:1.7.3")
implementation("org.jetbrains.kotlinx:kotlinx-coroutines-play-services:1.7.3")

</details>

