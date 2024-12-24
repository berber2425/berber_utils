# Berber Utils

Berber platformu için utility fonksiyonlar, extensionlar, controllerler ve widgetler paketi.

## Özellikler

- Extension metodları

  - String extensions
  - DateTime extensions
  - List extensions
  - Map extensions
  - BuildContext extensions
  - Widget extensions

- Utility fonksiyonlar

  - Format helpers
  - Validation helpers
  - Platform helpers
  - File helpers
  - Network helpers

- Custom Controllerler

  - Form controllers
  - Input controllers
  - Animation controllers
  - Navigation controllers
  - State controllers

- Custom Widgetler
  - Input widgets
  - Button widgets
  - Card widgets
  - List widgets
  - Dialog widgets
  - Loading widgets
  - Error widgets

## Teknik Detaylar

### Kullanılan Teknolojiler

- Flutter
- Dart

### Geliştirme Ortamı Gereksinimleri

- Flutter SDK
- VS Code veya Android Studio
- Git

### Kurulum

1. `pubspec.yaml` dosyanıza bağımlılığı ekleyin:

```yaml
dependencies:
  berber_utils:
    git:
      url: https://github.com/berber2425/berber_utils.git
      ref: main
```

2. Bağımlılıkları yükleyin:

```bash
flutter pub get
```

## Proje Yapısı

```
lib/
  ├── src/
  │   ├── extensions/     # Extension metodları
  │   ├── utils/         # Utility fonksiyonlar
  │   ├── controllers/   # Custom controllerler
  │   └── widgets/       # Custom widgetler
  └── berber_utils.dart  # Ana paket dosyası
```

## Kullanım

```dart
import 'package:berber_utils/berber_utils.dart';

// Extension kullanımı
final formattedDate = DateTime.now().toFormattedString();
final slugifiedText = "Örnek Başlık".toSlug();

// Utility fonksiyon kullanımı
final isValidEmail = BerberValidators.email("test@example.com");
final fileSize = BerberFileUtils.getReadableSize(1024);

// Controller kullanımı
final formController = BerberFormController();
final inputController = BerberInputController();

// Widget kullanımı
BerberButton(
  text: "Kaydet",
  onPressed: () => print("Tıklandı"),
);

BerberCard(
  title: "Başlık",
  content: "İçerik",
);
```

## Katkıda Bulunma

1. Fork yapın
2. Feature branch oluşturun (`git checkout -b feature/amazing-feature`)
3. Değişikliklerinizi commit edin (`git commit -m 'feat: add amazing feature'`)
4. Branch'inizi push edin (`git push origin feature/amazing-feature`)
5. Pull Request oluşturun
