---
title: Algorithm Intercomparison
---

APEx facilitates algorithm intercomparison exercises, enabling the benchmarking of various algorithms against each
other, providing a quality metric for EO services that implement the same capability. This aids end users in making
informed decisions about which algorithm to choose.

Additionally, APEx assists in identifying the algorithms that would most benefit from cloudification or enhancement,
ensuring that only the most effective and efficient tasks are pursued.

The intercomparison activities are currently under development and will continue to evolve throughout the APEx project,
as it relies on APEx instantiation services and propagation services to provide the necessary tools and user interfaces
for conducting intercomparison exercises.

## Examples

### Intercomparison of Sentinel-1 backscatter computation

The APEx framework allows to simplify intercomparison by offering different implementations of the same algorithm
through the same interface. One such example is Sentinel-1 backscatter computation, for which there are three openEO
implementations, all accessible via the `sar_backscatter` openEO process on different openEO backends:

| Backend    | Implementation                             |
|------------|--------------------------------------------|
| EODC       | Sentinel-1 toolbox 'SNAP' implementation   |
| CDSE       | Orfeo implementation                       |
| Terrascope | A custom implementation on the Sentinelhub |

While all three implementations implement `sar_backscatter`, they may vary in the range of parameters they accept.
Therefore, the range of supported parameters becomes an important point of comparison, alongside the cost specified in
platform credits and the correctness of the results.

## Call for service providers

APEx is looking for a first category of algorithms to be intercompared. If you have an algorithm, consider onboarding it
using the APEx [Toolbox Cloudification](./toolboxcloud.md) support, and request your peers to do the same so that a first
intercomparison can be initiated.

If you believe your implementation outperforms one currently available in the APEx catalog, feel free to contact us.
We will further evaluate your case to determine if you have a potential candidate for intercomparison.
