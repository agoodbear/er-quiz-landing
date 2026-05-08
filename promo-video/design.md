# 急專大補帖 v2 — Promo Video Design

## Mood

暖調教學感、醫學嚴謹但不冰冷、像翻開一本好讀的考試書。
受眾：準備急診專科考試的住院醫師、年輕主治。
情緒：放心、被理解、想開始刷題。

## Palette

| Token | Hex | Use |
| --- | --- | --- |
| `bg-cream` | `#FBF7EE` | 主背景（米黃，紙感） |
| `bg-card` | `#FFFFFF` | 卡片底 |
| `ink-deep` | `#1E3A5F` | 主標題、重點數字（深藍） |
| `ink-mid` | `#5A6478` | 內文 |
| `ink-soft` | `#8B92A3` | 標籤、註解 |
| `accent-coral` | `#F08C5A` | 強調、CTA、選中態（粉橘） |
| `accent-gold` | `#D4A047` | 次要 accent、徽章（金） |
| `accent-mint` | `#6BAA82` | 正確 / 通過（薄荷綠） |
| `border-warm` | `#E8DFD0` | 卡片邊框、分隔線（暖灰） |

## Typography

- Headlines: `Noto Sans TC` 700/900 (中文) + `Inter` 700 (英數)
- Body: `Noto Sans TC` 400/500 + `Inter` 500
- Numbers: `Inter` 800 with `font-variant-numeric: tabular-nums`
- Sizes: 顯示 110-160px、副標 42-56px、卡片標題 36-44px、卡片內文 24-28px

## Corners & Density

- Cards: `border-radius: 20px`
- Pills / badges: `border-radius: 999px`
- Padding range: 32-72px
- Gap range: 16-32px

## Depth

- Subtle layered: 卡片用 `0 12px 32px rgba(30, 58, 95, 0.08)`
- 不用 neon glow、不用 sci-fi 光暈

## Motion

- Eases: `power3.out` 進場、`expo.out` 大字進場、`back.out(1.4)` 卡片彈入、`power2.in` 退場（最後一幕才用）
- 進場時長：0.5-0.9s，疊著 stagger 0.08-0.15s
- 永遠不用 `repeat: -1`

## Avoid

- 純黑底、霓虹色、賽博龐克、玻璃擬態
- 全螢幕線性漸層（米黃底已暖，疊漸層會髒）
- 簡體字、大陸用語
- 使用 emoji 代替 icon（用 Lucide 風格 SVG）
