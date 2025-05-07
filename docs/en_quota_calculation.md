# Quota & API Setup (English)

## 1. Enable YouTube Data API v3
1. Open **Google Cloud Console** and create / select a project.  
2. **APIs & Services → Enable APIs & Services** → search *“YouTube Data API v3”* → **Enable**.  
3. **Credentials → Create credentials → API key** – copy the key.

## 2. Free daily quota
| Method | Units |
|--------|------:|
| `search.list` | 100 |
| `videos.list` | 1 |
| `liveChatMessages.list` | ~5 |

Every project starts with **10 000 units / 24 h**.

## 3. 4‑hour stream maths
```
startup  = 2×search + videos   = 201 u
chat     = 4h × 3600/8s × 5 u ≈ 9000 u
TOTAL    ≈ 9201 u (<10 000)
```

## 4. Need more?
Ask for a quota increase in **Quotas → Request increase** (50 k – 100 k).  
Google only charges if you exceed 10 k units in one day.
