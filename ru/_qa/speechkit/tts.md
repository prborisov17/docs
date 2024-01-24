# Синтез речи (TTS)

#### Как озвучивать длинные тексты? {#long-texts}

Чтобы озвучить большой текст, разбейте его на части любым удобным для вас способом. [Максимальный размер](../../{{ speechkit-slug }}/concepts/limits.md#speechkit-limits) запросов на синтеза речи составляет 5000 символов.

#### Как настроить ударения и произношение? {#tts-stress-pronunciation}

Чтобы скорректировать произношение отдельных слов и текста в целом, воспользуйтесь разметкой [SSML](../../{{ speechkit-slug }}/tts/markup/ssml.md) или [TTS](../../{{ speechkit-slug }}/tts/markup/tts-markup.md).

#### Как добавить паузу в тексте? {#add-pause}

Чтобы поставить паузу в тексте, используйте [TTS-разметку](../../speechkit/tts/markup/tts-markup#markup-elements). В скобках укажите длительность паузы в миллисекундах. Пауза появится в тех местах, где вы поставите тег. Например: `Начало sil<[3000]> продолжение через 3 секунды`.

#### Запрос cURL не работает в Windows PowerShell {#curl-powershell}

В терминале Windows PowerShell команда `curl` является псевдонимом системного вызова [Invoke-WebRequest](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.utility/invoke-webrequest). 

В документации {{ yandex-cloud }} примеры вызовов API даны в синтаксисе командной оболочки Bash. Вы можете запустить эти примеры без изменений в консоли Linux, терминале macOS или терминале WSL Windows 10 и выше. Чтобы запустить примеры в Windows PowerShell, потребуется их переработать самостоятельно. Подробнее о соответствии команд Bash и Powershell и советы см. в разделе [{#T}](../../overview/concepts/console-syntax-guide.md).

#### Из чего складывается стоимость синтеза? {#tts-cost}

Примеры расчета стоимости использования, правила тарификации и актуальные цены смотрите в разделе [{#T}](../../{{ speechkit-slug }}/pricing.md).
