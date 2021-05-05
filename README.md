# ПАТИХАУС [в разработке]
Android-приложение для организации и поиска вечеринок

## Описание
Патихиус решает задачи для двух основных ролей пользоватей, фигурирующих на развлекательных мероприятиях: **организатора** и **участника**.

* Как **организатор**, вы можете создать любое развлекательное мероприятие (выезд на шашлыки, поиск компании для посещения концерта/боулинга/кинотеатра и т.п.), координировать и оповещать участников
* Как **участник**, вы можете просматривать мероприятия, созданные другими организаторами, читать их описания, записываться на участие

## Предварительный дизайн
То, как наше приложение будет выглядеть к концу разработки:

* Основной экран приложения со списком мероприятий

![Основной экран приложения со списком мероприятий](https://imgur.com/jE65Fjj.png)

* Экран мероприятий

![Экран мероприятий](https://i.imgur.com/Q0J7MzE.png)

## Запуск приложения
1. Клонируйте репозиторий в нужную папку на вашем компьютере с помощью команды:
  > git clone https://github.com/APT-EHOT/trpp_project.git
2. Запустите Android-эмулятор либо подключите физическое Android-устройство (предварительно включите режим разработчика и отладку по USB) к компьютеру с установленными ADB драйверами
3. Откройте терминал в корне папки клонированного проекта и выполните следующую команду:
  > gradle installDebug
4. Дождитесь окончания выполнения команды установки
5. На эмуляторе/физическом устройстве найдите в списке приложений приложение PartyHouse и запустите его

## Список зависимостей
```groovy
    implementation fileTree(dir: "libs", include: ["*.jar"])
    implementation "org.jetbrains.kotlin:kotlin-stdlib:$kotlin_version"
    implementation 'com.android.support:appcompat-v7:28.0.0'
    implementation 'com.android.support.constraint:constraint-layout:2.0.4'
    testImplementation 'junit:junit:4.12'
    androidTestImplementation 'com.android.support.test:runner:1.0.2'
    androidTestImplementation 'com.android.support.test.espresso:espresso-core:3.0.2'
```