# design_ass1
# Assignment 1 — Divide & Conquer Algorithms

## Architecture Notes
- Depth control: QuickSort recurses only into the smaller part; MergeSort uses cutoff + reusable buffer.
- Memory: MergeSort allocates one buffer and reuses; QuickSort and Select work in-place.
- Metrics: counters for depth, comparisons, moves; CSV export.

## Recurrence Analysis
- MergeSort: T(n) = 2T(n/2) + Θ(n) → Θ(n log n).
- QuickSort: average T(n) = T(n/2) + T(n/2) + Θ(n) → Θ(n log n); worst-case Θ(n²) but bounded by random pivot.
- Deterministic Select (MoM5): T(n) = T(n/5) + T(7n/10) + Θ(n) → Θ(n).
- Closest Pair: T(n) = 2T(n/2) + Θ(n) → Θ(n log n).

## Plots
(time vs n, depth vs n) — вставить PNG из matplotlib.

## Constant Factors
Cache effects, branch mispredictions, JVM GC influence runtime.

## Summary
Theory matches practice in growth rates, small differences from constants.

