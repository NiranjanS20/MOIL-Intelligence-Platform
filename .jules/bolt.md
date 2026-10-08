## 2024-05-19 - [Memoizing derived state from hover interactions]
**Learning:** Frequent hover state changes (`hoveredMineId`) trigger component re-renders that unnecessarily re-run derived array filtering calculations.
**Action:** When components have frequent interaction state updates (like hovers or active selections), ensure expensive or list-based derived calculations are wrapped in `useMemo` to skip re-processing static arrays.
