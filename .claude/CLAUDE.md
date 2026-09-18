# Global instructions

## Comments
Keep comments short and on topic. They only need to communicate what is needed to future developers.

## Testing

Use `pytest.mark.parametrize` (or the equivalent in other test frameworks) to combine
test functions that share the same assertion shape and differ only in input/expected
data, rather than writing a near-duplicate test function per case. Give each case a
descriptive `id`/label. Keep separate test functions only for cases that exercise a
genuinely different code path (different constructor arguments, a different method,
aggregation behavior across multiple inputs), not just different data through the same
path.
