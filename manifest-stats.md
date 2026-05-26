## Manifest status

![ops](https://img.shields.io/badge/ops-137-blue) ![implemented](https://img.shields.io/badge/implemented-126%20%2F%20137%20%2892%25%29-brightgreen) ![spec--only](https://img.shields.io/badge/spec--only-11-orange)

### Per-family coverage

| Family | Implemented | Spec-only | Total | Progress | Workloads |
| --- | ---: | ---: | ---: | --- | ---: |
| `attention` | 16 | 0 | 16 | `██████████` 100% | 71 |
| `convolution` | 0 | 6 | 6 | `░░░░░░░░░░` 0% | 40 |
| `elementwise` | 66 | 5 | 71 | `█████████░` 93% | 142 |
| `moe` | 11 | 0 | 11 | `██████████` 100% | 74 |
| `normalization` | 12 | 0 | 12 | `██████████` 100% | 50 |
| `reduction` | 19 | 0 | 19 | `██████████` 100% | 47 |
| `scan` | 2 | 0 | 2 | `██████████` 100% | 4 |

### Spec coverage

| Field | Coverage |
| --- | ---: |
| `ref_api` | 137 / 137 (100%) |
| `roofline` (func or flops+bytes) | 137 / 137 (100%) |
| `source.kernel_map` | 103 / 137 (75%) |
| `source.bench_manifest_driven` | 27 / 137 (20%) |

**Workloads:** 428 total — 3.00 per implemented op.

### Conformance gaps

- Implemented ops without `kernel_map`: **34**
- Implemented ops without `roofline`: **0**
- Implemented ops without `source.bench_manifest_driven`: **99**
- Implemented ops with fewer than two workloads: **0**

<details><summary>Spec-only ops (11)</summary>

| | | |
| --- | --- | --- |
| `AlibiFwdOp` | `Conv1dBiasFwdOp` | `Conv1dFwdOp` |
| `Conv2dBiasFwdOp` | `Conv2dFwdOp` | `Conv3dBiasFwdOp` |
| `Conv3dFwdOp` | `GeluAndMulFwdOp` | `GeluTanhAndMulFwdOp` |
| `SiluAndMulFwdOp` | `SinusoidalFwdOp` |  |

</details>
