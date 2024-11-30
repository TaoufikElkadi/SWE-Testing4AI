# SWE-Testing4AI

## Biased Model
We created a biased model through three key mechanisms:

1. Feature Selection:
- Used demographic features (persoon_, wijk_, buurt_, relatie_)
- Created explicit age groups (young/middle/old)
- Added district risk scores

2. Sample Weighting:
- Young people: 2x weight
- Middle/old: 0.5x weight
- High-risk districts: 2x weight
- Low-risk districts: 0.5x weight

3. Combined Bias:
- Young people in high-risk areas get 4x weight (2 * 2)
- Older people in low-risk areas get 0.25x weight (0.5 * 0.5)

The results show clear discriminatory patterns:

1. Young people in high-risk districts face highest check rate (28.1%)
2. Young people in low-risk districts still face high checks (20.8%)
3. Middle/old age groups face very low check rates (1-2%)
4. High-risk districts increase checks by ~35% for young people
5. District risk has minimal impact on middle/old groups

This demonstrates the model's bias against young people, especially those in "high-risk" districts, while largely ignoring older residents regardless of location.
