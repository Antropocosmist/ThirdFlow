# Third Flow — BTC Tracker & Racer

Сайт с ценой биткоина в реальном времени, графиком, кошельками и игрой-гонкой.

## Возможности

- **BTC/USDT** — цена в реальном времени через Binance WebSocket
- **1M Chart** — график цены за последнюю минуту (Canvas)
- **MetaMask** — подключение, баланс ETH, сеть
- **Keplr** — подключение, баланс ATOM (Cosmos Hub)
- **🏎️ BTC Racer** — гоночная игра: дорога поворачивает в зависимости от цены BTC (вверх → вправо, вниз → влево)
- **🏆 Leaderboard** — топ-10 результатов, сохраняется в localStorage

## Как запустить

```bash
python3 -m http.server 8080 --bind 0.0.0.0
```

Открыть `http://127.0.0.1:8080`

> Расширения кошельков (MetaMask, Keplr) требуют HTTP(S) — не работают через `file://`.

## Управление игрой

| Клавиша | Действие |
|---------|----------|
| ← → / A D | Поворот машины |
| Enter (Game Over) | Сохранить результат / Новая игра |

## Технологии

- HTML5 Canvas
- Binance WebSocket API (BTC/USDT)
- Cosmos REST API (баланс ATOM)
- MetaMask EIP-1193
- Keplr Wallet API
- localStorage (лидерборд)
