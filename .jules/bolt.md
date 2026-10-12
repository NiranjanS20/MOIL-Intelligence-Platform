## 2024-10-12 - Single-Pass Loop Optimization in React
**Learning:** Found an anti-pattern where a component with multiple derived state variables from a single dataset performed O(n * m) passes using multiple `.filter()` calls. Wrapping them in a single O(n) pass inside `useMemo` reduced unnecessary iterations drastically.
**Action:** When calculating multiple counts and filtered views from the same source dataset, combine them into a single loop to minimize CPU overhead on state changes.
