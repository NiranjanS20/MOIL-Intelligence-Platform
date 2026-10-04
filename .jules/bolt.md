## 2024-10-04 - [Memoization in MineWorkspace]
**Learning:** Derived state in large React components (`MineWorkspace.tsx`) is recalculated on every render.
**Action:** Use `useMemo` to memoize expensive derived state computations to prevent unnecessary recalculations.
