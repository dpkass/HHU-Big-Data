# Big Data (Data Science II)

**Author:** Taha El Amine Kassabi\
**Course:** Data Science II (WS 2024/25)\
**Instructor:** Dr. Konrad Völkel\
**University:** Heinrich Heine University Düsseldorf (HHU)

---

## 📚 Overview

This repository collects my solutions to assignments from the *Data Science II* course at HHU.\
The focus is on **large-scale data processing**, **probabilistic algorithms**, and **scalable clustering** techniques.
Solutions were developed in Python, leveraging tools like **MRJob**, **NumPy**, **Scikit-learn**, and **NetworkX**.

---

## 📂 Repository Structure

```
Solutions/
├── Blatt 01 → Sparse matrix multiplication with MRJob
├── Blatt 02 → Jaccard similarity, shingling
├── Blatt 03 → MinHash, LSH, Enron mail similarity
├── Blatt 04 → LSH query engine, performance experiments
├── Blatt 05 → Bloom filters, Flajolet-Martin sketching
├── Blatt 06 → Graph loading, PageRank (Google web graph)
├── Blatt 07 → Wikipedia graph, spectral ranking
├── Blatt 08 → Graph streaming analysis
├── Blatt 09 → GMM clustering (NYC Taxi data)
├── Blatt 10 → BFR clustering
└── requirements.txt
```

---

## 🧠 Topics Covered

| Blatt | Algorithms / Methods                                 | Dataset                         |
|-------|------------------------------------------------------|---------------------------------|
| 01    | Sparse matrix multiplication, MapReduce              | Synthetic                       |
| 02    | Jaccard similarity, shingles                         | Kijiji Rome rentals             |
| 03    | MinHash signatures, LSH buckets                      | Enron email dataset             |
| 04    | Query tuning, LSH runtime evaluation                 | Enron email dataset             |
| 05    | Bloom filter, hash functions, Flajolet-Martin sketch | Synthetic streams               |
| 06    | PageRank, NetworkX, power iteration                  | Google WebGraph (snap.stanford) |
| 07    | Spectral ranking, eigenvectors                       | Wikipedia page graph            |
| 08    | Graph streaming, custom sketching                    | Wikipedia edge stream           |
| 09    | Gaussian Mixture Models, EM                          | NYC Taxi 2023 subset            |
| 10    | BFR clustering, large-scale partitioning             | NYC Taxi 2023 subset            |

---

## 📁 Setup

```bash
pip install -r requirements.txt
```

---

## 🚀 Usage

```bash
# Jupyter notebooks:
cd Solutions/Blatt\ 05
jupyter lab

# Standalone Python scripts:
python Solutions/Blatt09/bfr_clustering.py
```

---

## 📊 Notes

- MapReduce implementations use **MRJob**.
- Graph tasks rely on **NetworkX**; large datasets preprocessed to sparse format.
- Clustering solutions benchmark **BFR** against **GMM** (with covariance comparison).
- All implementations written from scratch. LLMs were used for research/reference only.
