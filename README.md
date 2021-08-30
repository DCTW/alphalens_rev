# Adapted from Alphalens


## Changes

- Add long/short attribute as `_type` in `utils.get_clean_factor_and_forward_returns`
- Add intraday plots of cumulative returns in given periods
- Calculate after-fee returns and change all cumulative returns from `cumprod` to `cumsum`

## Examples
Simple examples are located in `examples/`

## Solutions of warnings and errors
- Warnings:
```
import warnings
warnings.filterwarnings('ignore')
```
- Errors:
``` sh
def _validate_frequency(cls, index, freq, **kwargs):
    return None

pd.core.arrays.datetimelike.DatetimeLikeArrayMixin._validate_frequency = _validate_frequency

```
