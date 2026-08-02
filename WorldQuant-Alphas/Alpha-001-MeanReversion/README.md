# Alpha #1 - Submitted to WorldQuant BRAIN

- **Date Submitted:** August 2, 2026
- **Formula:** ts_decay_linear(group_neutralize(rank(-1 * (vwap - ts_mean(vwap, 5)) / ts_std_dev(vwap, 5)) * rank(volume / ts_mean(volume, 20)), industry), 5)
- **Rank:** 29,578
- **Score:** 1,935
- **Level:** Bronze
- **Universe:** USA/D1/TOP3000

**Strategy Logic (Plain English):**
This code works by hunting for stocks that are experiencing a sharp, sudden price drop alongside a massive spike in trading volume, which usually signals a moment of intense market panic. Capturing these extreme moments is important because they often create a "slingshot" effect where the stock quickly bounces back up to its normal price, allowing your strategy to lock in highly reliable profits.

<img width="1758" height="904" alt="Screenshot 2026-08-02 214416" src="https://github.com/user-attachments/assets/0271f80d-f61f-436a-b030-4fdf9bafded5" />
