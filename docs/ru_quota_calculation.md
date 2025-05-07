# Квоты и настройка API (Русский)

## 1. Включить YouTube Data API v3
1. В **Google Cloud Console** создайте или выберите проект.  
2. **APIs & Services → Enable APIs & Services** → найдите *«YouTube Data API v3»* → **Enable**.  
3. **Credentials → Create credentials → API key** – скопируйте ключ.

## 2. Бесплатный лимит
| Метод | Юниты |
|-------|------:|
| `search.list` | 100 |
| `videos.list` | 1 |
| `liveChatMessages.list` | ~5 |

Каждый проект получает **10 000 unit / сутки**.

## 3. 4‑часовой стрим
```
Старт     = 201 u
Чат       = 4 ч × 3600/8 c × 5 u ≈ 9000 u
ИТОГО     ≈ 9201 u (<10 000)
```

## 4. Нужно больше?
В **Quotas** нажмите *Request increase* и запросите 50–100 k.  
Платить начнёте, только если превысите 10 k unit за сутки.
