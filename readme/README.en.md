<div align="center">


# Course Notes

**Xi'an Jiaotong University · China University of Petroleum (Beijing)** — lecture notes and exam review materials, typeset in LaTeX

[简体中文](/README.md) | **English** | [繁體中文](/readme/README.zh_TW.md)

**Typeset in LaTeX** · **PDF ready to read** · **Continuously updated**

</div>

## About

This repository collects course notes and exam review materials from my undergraduate and graduate studies. The text is written in LaTeX, and the compiled PDFs can be downloaded directly.

Everything is shared for free and updated continuously. If you find it useful, a **Star** ⭐ is appreciated.

## Contents

| Course                                         | Institution / Term        | Content                                                      | Pages | Files                                                        |
| :--------------------------------------------- | :------------------------ | :----------------------------------------------------------- | :---: | :----------------------------------------------------------- |
| Technical Economics and Engineering Management | CUPB · Fall 2024          | 8 chapters + exam analysis                                   |  117  | [PDF](/%E6%8A%80%E6%9C%AF%E7%BB%8F%E6%B5%8E%E4%B8%8E%E5%B7%A5%E7%A8%8B%E7%AE%A1%E7%90%86.pdf) · [LaTeX](/%E6%8A%80%E6%9C%AF%E7%BB%8F%E6%B5%8E%E4%B8%8E%E5%B7%A5%E7%A8%8B%E7%AE%A1%E7%90%86/) |
| Database Course Final Review 2026              | Xi'an Jiaotong University | Fill-in / multiple choice / short answer / design questions, answers included |  25   | [PDF](/xjtu%E7%A0%94%E7%A9%B6%E7%94%9F%E6%95%B0%E6%8D%AE%E5%BA%93%E8%AF%BE%E7%A8%8B%E6%9C%9F%E6%9C%AB%E5%A4%8D%E4%B9%A0%E9%A2%982026.pdf) · [LaTeX](/xjtu%E7%A0%94%E7%A9%B6%E7%94%9F%E6%95%B0%E6%8D%AE%E5%BA%93%E8%AF%BE%E7%A8%8B%E6%9C%9F%E6%9C%AB%E5%A4%8D%E4%B9%A0%E9%A2%982026.tex) |

## Notes in detail

### Technical Economics and Engineering Management (117 pages)

1. Introduction
2. Composition of cash flows
3. Equivalence calculation of funds
4. Determination of the benchmark discount rate
5. Indicators for evaluating economic results
6. Methods for evaluating economic results
7. Uncertainty and risk analysis
8. Financial evaluation of projects
9. Exam analysis: question types and chapter weighting

### Database Course Final Review 2026 (25 pages)

| Question type                       | Count |
| :---------------------------------- | ----: |
| Fill-in-the-blank                   |    21 |
| Multiple choice (with explanations) |    29 |
| Short answer                        |    16 |
| Comprehensive design                |     2 |

Topics covered: semi-structured data models, OEM / RDF / ontologies, Bloom and Cuckoo filters, skip lists, LSM trees, cloud-native and AI-native databases, RAG, vector search, B+ trees, and join cost estimation. All questions come with reference answers.

## Repository structure

```text
Course-Notes/
├── README.md
├── readme/                              # translations
│   ├── README.en.md
│   ├── README.zh_CN.md
│   └── README.zh_TW.md
├── 技术经济与工程管理.pdf                # 117 pages
├── 技术经济与工程管理/
│   ├── main.tex                         # main file
│   ├── chapter1/ … chapter8/            # chapter sources
│   ├── 考试分析/                         # exam analysis
│   ├── image/                           # figures
│   └── elegantbook.cls
├── xjtu研究生数据库课程期末复习题2026.tex
└── xjtu研究生数据库课程期末复习题2026.pdf
```

## Building from source

A full TeX distribution (TeX Live or MiKTeX) is required; compile with **XeLaTeX**.

```bash
# Technical Economics and Engineering Management
cd 技术经济与工程管理
xelatex main.tex
xelatex main.tex        # run twice to resolve the table of contents

# Database final review
xelatex xjtu研究生数据库课程期末复习题2026.tex
```

- `main.tex` uses the `ctexbook` class and depends on `ctex`, `amsmath`, `fancyhdr`, `longtable`, etc.
- The review document uses `ctexart` with `tcolorbox` (answer boxes), `enumitem`, and `booktabs`.
- The B+ tree figures for the review document live in `figs/` (8 PNG files) and must sit next to the `.tex` file.

## Usage & disclaimer

- All materials are **free to share**; **selling them in any form is prohibited**.
- Content is compiled from lecture slides, lectures, and public videos on Bilibili, for study and exchange only. Rights holders may contact the author for removal.
- Corrections and additions are welcome via Issues or Pull Requests.
- Notes sharing only — no tutoring or Q&A support.
- The author reserves the right of interpretation.

## Contact

- Email: `zhangziyan527@163.com` (alternate: `ZSDZZY2022@163.com`)
- GitHub: [@ZZY1234321](https://github.com/ZZY1234321)

<sub>Last updated: 2026-11-14 · Added "Database Course Final Review 2026"</sub>
