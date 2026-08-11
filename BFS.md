Day 01(04/08/2026): Summary:

Time complexity - Measures the time taken to run a program depending on the input size.

Slowest to fastest order:

O(2^n) --> Exponential O(n!) --> Factorial O(n^3) --> Cubic O(n^2) --> Square/Quadratic (Outer loop depends on the inner loop of range n.) O(nlogn) --> Logrithmic (Outer loop of range n depends on inner loop of range n/2.) O(n) --> Linear (depends on the range of n.) O(1) --> Constant The Three Notations:

Upper Bound - This represents the worst case. The algorithm will not grow faster than this rate.

Lower Bound - This represents the best case. The algorithm will not grow slower than this rate.

Tight Bond - This represents the constant. The algorithm grows exactly at that rate.

Steps to find the time complexity from a code:

Drop/Remove Constants. Keep the Dominant Term. Nested Loops Multiply.
