## About this repository

This repository provides the Jupyter notebooks, input data, and simulation results for the computational experiments reported in the following manuscript:

**Finite-size boundary corrections to the Beardwood–Halton–Hammersley formula for the traveling salesman problem**  
Daisuke Hasegawa, The University of Tokyo.

This repository investigates a perimeter-based finite-size correction for the expected Euclidean traveling salesman problem (TSP) tour length. Toroidal boundary conditions are used as a boundary-free reference to separate interior and boundary contributions. The study evaluates two models:

**PC-Const:** `E[L_N] ≈ beta * sqrt(N * A) + gamma * P`
**PC-FN:** `E[L_N] ≈ beta * sqrt(N * A) + (gamma_inf + c / sqrt(N)) * P`

Here, `N` is the number of uniformly sampled demand points, `A` is region area, and `P` is its perimeter.

## Files

The notebooks are in `notebook/`, geographic input data in `data/`, and saved simulation results, tables, and figures in `output/`. Run the notebooks from the `notebook/` directory.

## Geographic data and attribution

The real-world analysis uses small-area boundaries and household counts from the **2020 Population Census of Japan**, made available by the **Statistics Bureau of Japan** through the e-Stat statistical GIS service: https://www.e-stat.go.jp/gis . The source records were aggregated and processed to construct ten administrative districts of Kawaguchi City. `data/district.csv` provides the small-area-to-district mapping and is read with CP932 encoding in the notebook.

**Attribution:** “2020 Population Census of Japan,” Statistics Bureau of Japan, obtained via e-Stat; processed by the author. The supplied geographical data and any derived data remain subject to the applicable original-source terms. See [e-Stat terms of use](https://www.e-stat.go.jp/terms-of-use) and [GIS terms](https://www.e-stat.go.jp/gis-terms). The MIT license below does **not** relicense third-party geographic or census data.

## License

The original research code is provided under the [MIT License](LICENSE).
