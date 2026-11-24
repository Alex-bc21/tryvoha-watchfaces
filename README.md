# Тривога поруч — циферблаты Wear OS

<!-- download-and-share -->
Tryvoha Poruch: Emerald Vault, Obsidian Prism and Sapphire Flow watch faces for Wear OS 6, built with Watch Face Format 4.

### Скачать и установить

- **[EmeraldVaultWatchFace-1.3.0.apk](https://github.com/Alex-bc21/tryvoha-watchfaces/releases/download/v1.3.0/EmeraldVaultWatchFace-1.3.0.apk)**
- **[ObsidianPrismWatchFace-1.2.0.apk](https://github.com/Alex-bc21/tryvoha-watchfaces/releases/download/v1.3.0/ObsidianPrismWatchFace-1.2.0.apk)**
- **[SapphireFlowWatchFace-1.2.0.apk](https://github.com/Alex-bc21/tryvoha-watchfaces/releases/download/v1.3.0/SapphireFlowWatchFace-1.2.0.apk)**

[Полные исходники](https://github.com/Alex-bc21/tryvoha-watchfaces/releases/download/v1.3.0/WatchFaces-1.3.0-source.zip) · [Все версии и контрольные суммы](https://github.com/Alex-bc21/tryvoha-watchfaces/releases)

APK предназначены для часов Wear OS 6, не для телефона. Способ установки и отдельный поставщик статуса тревоги описаны ниже.

Это предварительные версии для ознакомления и тестирования. Для скачивания публичных файлов регистрация на GitHub не нужна.

**Поделиться:** отправьте [ссылку на этот проект](https://github.com/Alex-bc21/tryvoha-watchfaces) — здесь будут актуальное описание и ссылки на версии. [Сообщить об ошибке](https://github.com/Alex-bc21/tryvoha-watchfaces/issues).
<!-- /download-and-share -->

Три циферблата с разными оформлением и пакетами:

- Emerald Vault 1.3.0 — com.emeraldvault.watchface.
- Obsidian Prism 1.2.0 — com.obsidianprism.watchface.
- Sapphire Flow 1.2.0 — com.sapphireflow.watchface.

[Скачать все APK и исходники](https://github.com/Alex-bc21/tryvoha-watchfaces/releases/tag/v1.3.0).

Предварительная архивная подборка: Watch Face Format 4, **Wear OS 6 / API 36**. Эти APK предназначены для часов, а не телефона. Это восстановленные версии сентября 2026 года; более поздняя подготовленная Play-сборка 1.4.0 в подборку не входит.

Для точки тревоги на часах нужен отдельный поставщик `com.sasha.tryvohaporuch/.complication.AlarmComplicationService`. Его APK не включён. Исходники поставщика находятся в модуле wear [проекта виджета](https://github.com/Alex-bc21/tryvoha-poruch-android). Установка только циферблата не создаёт службу получения статуса тревоги. Индикатор не заменяет официальное оповещение.

## Сборка и установка

`WatchFaces-1.3.0-source.zip` содержит все три проекта, графику и лицензии шрифтов. Нужны Android SDK Platform 36, Build Tools 36.0.0, JDK и Bash. Задайте ANDROID_SDK_ROOT и выполните `bash build-all-apks.sh`. Оригинальный ключ не включён: скрипт создаст ваш локальный ключ. APK с иной подписью не обновит оригинальный поверх установленного.

На подключённых часах: `adb install -r EmeraldVaultWatchFace-1.3.0.apk`, затем выберите циферблат в настройках часов. Можно установить все три независимо.

Проверены подписи оригинальных APK, версии, ZIP и компиляция ресурсов каждого проекта. Работа анимаций, AOD и статусов на физических часах при этой публикации не проверялась. [Руководство](USER-GUIDE.md), [данные](PRIVACY.md), [проверка](VERIFICATION.md). Лицензии шрифтов сохранены в docs внутри проекта.

