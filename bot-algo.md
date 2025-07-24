How are tiles handled?
- Tiles are rotated and evaluated for placement based on river continuity, adjacency to existing tiles, and avoidance of problematic U-turns. A heuristic scores nearby open positions by connection density and distance from center.

How are meeples placed?
- Meeples are placed only if there’s a preferred feature (city, monastery, road) with no existing claim. The bot prioritizes high-scoring features and avoids wasted placements.

How is this efficient?
- The bot limits the number of tile/rotation/position checks using a time cutoff and maximum trial count. It also uses fallback logic, avoids duplicate evaluations via caching (tried set), and prioritizes strategic positions.
