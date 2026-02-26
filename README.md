**[Slides on Data Collecting](https://www.canva.com/design/DAG2byRhzN4/kFebQSHbVgpsxHitZe8xyA/edit?utm_content=DAG2byRhzN4&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)**

## Executive Summary
This project investigates the "Lipstick Effect"—the behavioral economic theory that consumers pivot toward small luxuries during recessions. By correlating high-granularity retail data from Sephora with national indices like GDP and unemployment, I built a pipeline to identify early-warning indicators of economic shifts.

### Technical Workaround & Data Strategy
Facing strict bot-detection on the U.S. Sephora site, I engineered a strategic workaround to capture time-stamped reviews (a proxy for sales volume):
- **The Manual Capture:** Intercepted JSON network fetches via Chrome DevTools to bypass dynamic rendering and bot-blocks on the U.S. site.
- **The Malaysia Proxy:** Utilized Sephora’s Malaysia site—which features a simpler static architecture—to prototype and refine BeautifulSoup parsing logic.
- **U.S. Data Integrity:** While the logic was tested via the Malaysia proxy, the final metrics are grounded in U.S. reviews (filtered by "Originally posted on sephora.com") to maintain domestic economic validity.

### Key Insights & Reflection
This "many-hats" approach allowed me to move from a "black box" understanding of web architecture to a granular mastery of the data capture process. The resulting dataset enables a comparative exploration of the U.S. economic cycle, offering a unique, audited perspective on consumer behavior in relation to macroeconomic trends
