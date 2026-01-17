# 📋 Task Planlama Raporu

## 📌 Proje Bilgileri

| Alan | Değer |
|------|-------|
| **Proje Adı** | local-mind |
| **Platform** | iOS |
| **Oluşturulma Tarihi** | 2026-01-17 |
| **Agent** | Business Analyst |
| **Template** | [TEMPLATE-iOS] SwiftUI iOS 17+ Proje Şablonu |

---

## 📝 Proje Açıklaması

**Konsept:** Tamamen cihaz üzerinde çalışan, internet gerektirmeyen kişisel AI asistan. Not tutma, görev yönetimi ve basit soruları yanıtlama özellikleri.

**Hedef Kitle:** Gizlilik odaklı kullanıcılar, sık seyahat edenler, sınırlı internet erişimi olanlar

**Öne Çıkan Özellik:** Sıfır veri toplama garantisi, tamamen offline çalışma, özelleştirilebilir AI modelleri

**Teknoloji:** Apple Intelligence, Core ML, NaturalLanguage framework

**Monetizasyon:** Tek seferlik ödeme $9.99 veya $14.99

---

## 📊 Özet İstatistikler

| Metrik | Değer |
|--------|-------|
| **Toplam Task** | 14 |
| **SIRA Aralığı** | [SIRA-(-1)] → [SIRA-12] |
| **Tahmini PR Sayısı** | 14 |
| **Platform** | iOS 17+ |
| **Framework** | SwiftUI + SwiftData |
| **AI** | Apple Intelligence + Core ML |

---

## 📋 Task Listesi

| SIRA | Task Başlığı | Özet |
|------|--------------|------|
| -1 | GitHub Repo + Xcode Proje Setup | Repo oluşturma, template'den proje kurulumu |
| 0 | CI/CD Pipeline | GitHub Actions workflow, otomatik build/test |
| 1 | Design System | Colors, Typography, Spacing, Shadows |
| 2 | Core Components | Cards, Buttons, Inputs, Lists |
| 3 | SwiftData Models | Note, TaskItem, Conversation, Message, AppSettings |
| 4 | ViewModels | NotesVM, TasksVM, AIAssistantVM + Tests |
| 5 | Main Views + AI | TabView, Dashboard, Lists, AssistantView |
| 6 | Detail Views | Note/Task editors, Navigation |
| 7 | Settings | Preferences, Privacy, Data Management |
| 8 | Animations | Effects, Transitions, Haptics |
| 9 | Localization | Türkçe/İngilizce dil desteği |
| 10 | App Icons + Launch Screen | Branding, Launch animation |
| 11 | Apple Intelligence | NLP, Summarization, Smart suggestions |
| 12 | Final Integration | Testing, App Store hazırlığı |

---

## 📝 Task Detayları

### [SIRA-(-1)] GitHub Repo + Xcode Proje Setup

**Özet:** Local Mind iOS uygulaması için GitHub repository ve Xcode proje yapısını oluştur.

**Yapılacaklar:**
1. GitHub repo oluştur (kamilsevket/local-mind)
2. Template repodan Xcode yapısını çek
3. Proje adını LocalMind olarak değiştir
4. SwiftData container tanımla
5. İlk commit ve push

**Oluşturulacak Dosyalar:**
- `LocalMind.xcodeproj/`
- `LocalMind/App/LocalMindApp.swift`
- Tüm klasör yapısı

**Tamamlanma Kriterleri:**
- [ ] GitHub repo oluşturuldu
- [ ] Xcode projesi hazır
- [ ] SwiftData container tanımlı
- [ ] main branch'e push edildi

---

### [SIRA-0] CI/CD Pipeline (GitHub Actions)

**Özet:** Her PR'da otomatik build ve test çalıştıran GitHub Actions workflow.

**Yapılacaklar:**
1. `.github/workflows/ios.yml` oluştur
2. macOS 14 + Xcode 15.2 konfigürasyonu
3. Build ve test stepları
4. Branch protection rules

**Oluşturulacak Dosyalar:**
- `.github/workflows/ios.yml`

**Tamamlanma Kriterleri:**
- [ ] Workflow dosyası oluşturuldu
- [ ] CI SUCCESS çalışıyor
- [ ] Branch protection aktif

---

### [SIRA-1] Design System (Colors, Typography, Spacing)

**Özet:** Local Mind için özel tasarlanmış Design System - gizlilik odaklı, sakin, modern.

**Yapılacaklar:**
1. AppColors.swift - Purple/Teal gradients, semantic colors
2. AppTypography.swift - Rounded font sistemi
3. AppSpacing.swift - 4pt grid
4. AppShadows.swift - Elevation utilities

**Oluşturulacak Dosyalar:**
- `LocalMind/Theme/AppColors.swift`
- `LocalMind/Theme/AppTypography.swift`
- `LocalMind/Theme/AppSpacing.swift`
- `LocalMind/Theme/AppShadows.swift`

**Testler:**
- `LocalMindTests/AppColorsTests.swift`

**Tamamlanma Kriterleri:**
- [ ] Tüm theme dosyaları oluşturuldu
- [ ] Hex color extension çalışıyor
- [ ] Unit testler yazıldı

---

### [SIRA-2] Core Components (Cards, Buttons, Inputs)

**Özet:** Temel UI componentleri: Glass cards, modern buttons, text inputs.

**Yapılacaklar:**
1. GlassCard, FeatureCard, GradientCard
2. PrimaryButton, SecondaryButton, IconButton, FAB
3. AppTextField, SearchField, ChatInputField
4. NoteRow, TaskRow, SettingsRow
5. EmptyStateView, LoadingView

**Oluşturulacak Dosyalar:**
- `LocalMind/Components/GlassCard.swift`
- `LocalMind/Components/ModernCard.swift`
- `LocalMind/Components/AppButtons.swift`
- `LocalMind/Components/AppTextField.swift`
- `LocalMind/Components/ListComponents.swift`
- `LocalMind/Components/StateViews.swift`

**Tamamlanma Kriterleri:**
- [ ] Tüm component dosyaları oluşturuldu
- [ ] Design system kullanılıyor
- [ ] Interactive states çalışıyor

---

### [SIRA-3] SwiftData Models + Tests

**Özet:** Tüm data modelleri: Note, TaskItem, Conversation, Message, AppSettings.

**Yapılacaklar:**
1. Note model - tags, pinning, color support
2. TaskItem model - priorities, subtasks, due dates
3. Conversation & Message - AI chat history
4. AppSettings - user preferences
5. ModelContainer yapılandırması (offline only)

**Oluşturulacak Dosyalar:**
- `LocalMind/Models/Note.swift`
- `LocalMind/Models/TaskItem.swift`
- `LocalMind/Models/Conversation.swift`
- `LocalMind/Models/Message.swift`
- `LocalMind/Models/AppSettings.swift`

**Testler:**
- `LocalMindTests/NoteTests.swift`
- `LocalMindTests/TaskItemTests.swift`
- `LocalMindTests/ConversationTests.swift`
- `LocalMindTests/MessageTests.swift`

**Tamamlanma Kriterleri:**
- [ ] Tüm modeller @Model macro ile
- [ ] Relationships tanımlı
- [ ] Comprehensive testler yazıldı

---

### [SIRA-4] ViewModels + Tests

**Özet:** MVVM ViewModels: NotesViewModel, TasksViewModel, AIAssistantViewModel.

**Yapılacaklar:**
1. NotesViewModel - CRUD, search, filter, sort
2. TasksViewModel - priorities, due dates, subtasks
3. AIAssistantViewModel - chat management
4. LocalAIService placeholder

**Oluşturulacak Dosyalar:**
- `LocalMind/ViewModels/NotesViewModel.swift`
- `LocalMind/ViewModels/TasksViewModel.swift`
- `LocalMind/ViewModels/AIAssistantViewModel.swift`
- `LocalMind/Services/LocalAIService.swift`

**Testler:**
- `LocalMindTests/NotesViewModelTests.swift`
- `LocalMindTests/TasksViewModelTests.swift`
- `LocalMindTests/AIAssistantViewModelTests.swift`

**Tamamlanma Kriterleri:**
- [ ] @Observable macro kullanılıyor
- [ ] Full CRUD operations
- [ ] Filter/sort/search çalışıyor
- [ ] Mock AI service ile testler

---

### [SIRA-5] Main Views + AI Integration

**Özet:** Ana view'lar: MainTabView, DashboardView, Lists, AssistantView.

**Yapılacaklar:**
1. MainTabView - custom tab bar
2. DashboardView - stats, recent items
3. NotesListView - search, filter, sort
4. TasksListView - filter pills
5. AssistantView - chat interface

**Oluşturulacak Dosyalar:**
- `LocalMind/Views/Main/MainTabView.swift`
- `LocalMind/Views/Main/DashboardView.swift`
- `LocalMind/Views/Notes/NotesListView.swift`
- `LocalMind/Views/Tasks/TasksListView.swift`
- `LocalMind/Views/Assistant/AssistantView.swift`

**Tamamlanma Kriterleri:**
- [ ] Tab navigation çalışıyor
- [ ] Dashboard stats gösteriyor
- [ ] List views filter/search destekliyor
- [ ] Chat interface çalışıyor

---

### [SIRA-6] Detail Views + Navigation

**Özet:** Not ve görev detay/düzenleme ekranları.

**Yapılacaklar:**
1. NoteEditorView - create/edit with tags
2. NoteDetailView - read-only with actions
3. TaskEditorView - subtasks, due date, priority
4. FlowLayout for tags

**Oluşturulacak Dosyalar:**
- `LocalMind/Views/Notes/NoteEditorView.swift`
- `LocalMind/Views/Notes/NoteDetailView.swift`
- `LocalMind/Views/Tasks/TaskEditorView.swift`

**Tamamlanma Kriterleri:**
- [ ] Sheet presentations çalışıyor
- [ ] Create/Edit modes
- [ ] Delete confirmation

---

### [SIRA-7] Settings & Preferences

**Özet:** Ayarlar: AI model tercihleri, gizlilik, data management.

**Yapılacaklar:**
1. SettingsView - AI model selection, toggles
2. AboutView - feature highlights
3. PrivacyInfoView - privacy policy
4. DataManagementView - storage overview

**Oluşturulacak Dosyalar:**
- `LocalMind/Views/Settings/SettingsView.swift`
- `LocalMind/Views/Settings/AboutView.swift`
- `LocalMind/Views/Settings/PrivacyInfoView.swift`
- `LocalMind/Views/Settings/DataManagementView.swift`

**Tamamlanma Kriterleri:**
- [ ] AI preference seçimi
- [ ] Delete all data çalışıyor
- [ ] Privacy info görüntüleniyor

---

### [SIRA-8] Animations & Polish

**Özet:** Animasyonlar, geçiş efektleri, haptic feedback.

**Yapılacaklar:**
1. Animation presets (spring, ease, snappy)
2. Shimmer, pulse, floating effects
3. Custom transitions
4. HapticManager

**Oluşturulacak Dosyalar:**
- `LocalMind/Animations/AppAnimations.swift`
- `LocalMind/Animations/SkeletonLoading.swift`
- `LocalMind/Animations/TransitionEffects.swift`
- `LocalMind/Services/HapticManager.swift`

**Tamamlanma Kriterleri:**
- [ ] Animation modifiers çalışıyor
- [ ] Skeleton loading componentleri
- [ ] Haptic feedback entegre

---

### [SIRA-9] Localization (TR/EN)

**Özet:** Türkçe ve İngilizce dil desteği.

**Yapılacaklar:**
1. String Catalog oluştur
2. Tüm UI string'lerini localize et
3. L10n enum for type-safe access
4. Views'ı güncelle

**Oluşturulacak Dosyalar:**
- `LocalMind/Resources/Localizable.xcstrings`
- `LocalMind/Extensions/LocalizedStrings.swift`

**Testler:**
- `LocalMindTests/LocalizationTests.swift`

**Tamamlanma Kriterleri:**
- [ ] TR/EN çeviriler tamamlandı
- [ ] L10n enum kullanılıyor
- [ ] Tüm views güncellendi

---

### [SIRA-10] App Icons + Launch Screen

**Özet:** App icon seti ve launch screen.

**Yapılacaklar:**
1. App icon tüm boyutlarda
2. LaunchScreen.swift with animations
3. Color assets
4. App entry point güncelleme

**Oluşturulacak Dosyalar:**
- `LocalMind/Resources/Assets.xcassets/AppIcon.appiconset/`
- `LocalMind/Views/LaunchScreen.swift`
- Color assets

**Tamamlanma Kriterleri:**
- [ ] App icon tüm boyutlarda
- [ ] Animated launch screen
- [ ] Smooth transition to main app

---

### [SIRA-11] Apple Intelligence Integration

**Özet:** On-device AI: NLP, summarization, smart suggestions.

**Yapılacaklar:**
1. LocalAIService with NaturalLanguage framework
2. Intent analysis
3. Summarization
4. NoteAnalysisService
5. TaskSuggestionService

**Oluşturulacak Dosyalar:**
- `LocalMind/Services/LocalAIService.swift` (güncelle)
- `LocalMind/Services/WritingToolsService.swift`
- `LocalMind/Services/NoteAnalysisService.swift`
- `LocalMind/Services/TaskSuggestionService.swift`

**Testler:**
- `LocalMindTests/AIServiceTests.swift`
- `LocalMindTests/TaskSuggestionServiceTests.swift`
- `LocalMindTests/NoteAnalysisServiceTests.swift`

**Tamamlanma Kriterleri:**
- [ ] NLP-based responses
- [ ] Summarization çalışıyor
- [ ] Smart suggestions aktif
- [ ] Tamamen offline

---

### [SIRA-12] Final Integration & Testing

**Özet:** Tüm componentleri entegre et, comprehensive tests, App Store hazırlığı.

**Yapılacaklar:**
1. ContentView entry point
2. OnboardingView
3. Integration tests
4. UI tests
5. Performance tests
6. App Store metadata

**Oluşturulacak Dosyalar:**
- `LocalMind/Views/ContentView.swift`
- `LocalMind/Views/Onboarding/OnboardingView.swift`
- `LocalMindTests/IntegrationTests.swift`
- `LocalMindUITests/LocalMindUITests.swift`
- `LocalMindTests/PerformanceTests.swift`

**Tamamlanma Kriterleri:**
- [ ] Onboarding flow çalışıyor
- [ ] Tüm features entegre
- [ ] Integration tests geçiyor
- [ ] UI tests geçiyor
- [ ] Performance kabul edilebilir
- [ ] App Store metadata hazır

---

## 🔗 Bağımlılık Grafiği

```
[SIRA-(-1)] GitHub Repo
     │
     ▼
[SIRA-0] CI/CD Pipeline
     │
     ▼
[SIRA-1] Design System
     │
     ▼
[SIRA-2] Core Components
     │
     ├──────────────┬──────────────┐
     ▼              ▼              ▼
[SIRA-3]       [SIRA-4]       [SIRA-8]
Models         ViewModels     Animations
     │              │              │
     └──────┬───────┘              │
            ▼                      │
       [SIRA-5]                    │
       Main Views ◄────────────────┘
            │
     ┌──────┴──────┐
     ▼             ▼
[SIRA-6]      [SIRA-7]
Details       Settings
     │             │
     └──────┬──────┘
            ▼
       [SIRA-9]
       Localization
            │
            ▼
       [SIRA-10]
       Icons/Launch
            │
            ▼
       [SIRA-11]
       AI Integration
            │
            ▼
       [SIRA-12]
       Final Integration
            │
            ▼
         🎉 DONE!
```

---

## 📱 Dosya Yapısı (Tahmini)

```
LocalMind/
├── LocalMind.xcodeproj/
├── LocalMind/
│   ├── App/
│   │   └── LocalMindApp.swift
│   ├── Theme/
│   │   ├── AppColors.swift
│   │   ├── AppTypography.swift
│   │   ├── AppSpacing.swift
│   │   └── AppShadows.swift
│   ├── Components/
│   │   ├── GlassCard.swift
│   │   ├── ModernCard.swift
│   │   ├── AppButtons.swift
│   │   ├── AppTextField.swift
│   │   ├── ListComponents.swift
│   │   └── StateViews.swift
│   ├── Animations/
│   │   ├── AppAnimations.swift
│   │   ├── SkeletonLoading.swift
│   │   └── TransitionEffects.swift
│   ├── Models/
│   │   ├── Note.swift
│   │   ├── TaskItem.swift
│   │   ├── Conversation.swift
│   │   ├── Message.swift
│   │   └── AppSettings.swift
│   ├── ViewModels/
│   │   ├── NotesViewModel.swift
│   │   ├── TasksViewModel.swift
│   │   └── AIAssistantViewModel.swift
│   ├── Services/
│   │   ├── LocalAIService.swift
│   │   ├── WritingToolsService.swift
│   │   ├── NoteAnalysisService.swift
│   │   ├── TaskSuggestionService.swift
│   │   └── HapticManager.swift
│   ├── Views/
│   │   ├── ContentView.swift
│   │   ├── LaunchScreen.swift
│   │   ├── Main/
│   │   │   ├── MainTabView.swift
│   │   │   └── DashboardView.swift
│   │   ├── Notes/
│   │   │   ├── NotesListView.swift
│   │   │   ├── NoteDetailView.swift
│   │   │   └── NoteEditorView.swift
│   │   ├── Tasks/
│   │   │   ├── TasksListView.swift
│   │   │   └── TaskEditorView.swift
│   │   ├── Assistant/
│   │   │   └── AssistantView.swift
│   │   ├── Settings/
│   │   │   ├── SettingsView.swift
│   │   │   ├── AboutView.swift
│   │   │   ├── PrivacyInfoView.swift
│   │   │   └── DataManagementView.swift
│   │   └── Onboarding/
│   │       └── OnboardingView.swift
│   ├── Extensions/
│   │   └── LocalizedStrings.swift
│   └── Resources/
│       ├── Assets.xcassets/
│       └── Localizable.xcstrings
├── LocalMindTests/
│   ├── NoteTests.swift
│   ├── TaskItemTests.swift
│   ├── ConversationTests.swift
│   ├── MessageTests.swift
│   ├── NotesViewModelTests.swift
│   ├── TasksViewModelTests.swift
│   ├── AIAssistantViewModelTests.swift
│   ├── AIServiceTests.swift
│   ├── LocalizationTests.swift
│   ├── IntegrationTests.swift
│   └── PerformanceTests.swift
└── LocalMindUITests/
    └── LocalMindUITests.swift
```

---

## 🚀 Sonraki Adımlar

1. Agent Erman'ı bu proje için başlat
2. [SIRA-(-1)] task'ı otomatik başlayacak
3. Task'lar sırayla tamamlanacak
4. Her PR CI'dan geçecek
5. Proje bitince final review yapılacak

---

## 📊 Özellik Matrisi

| Özellik | Durum | Task |
|---------|-------|------|
| Offline AI | ✅ Planlı | SIRA-11 |
| Not Tutma | ✅ Planlı | SIRA-3, 4, 5, 6 |
| Görev Yönetimi | ✅ Planlı | SIRA-3, 4, 5, 6 |
| Apple Intelligence | ✅ Planlı | SIRA-11 |
| %100 Gizlilik | ✅ Planlı | Tüm task'lar |
| SwiftData | ✅ Planlı | SIRA-3 |
| Modern UI | ✅ Planlı | SIRA-1, 2, 8 |
| TR/EN Dil | ✅ Planlı | SIRA-9 |
| CI/CD | ✅ Planlı | SIRA-0 |
| Unit Tests | ✅ Planlı | SIRA-3, 4, 11 |
| UI Tests | ✅ Planlı | SIRA-12 |

---

*Bu rapor Agent Business Analyst tarafından otomatik oluşturulmuştur.*
*Tarih: 2026-01-17T12:15:00Z*
