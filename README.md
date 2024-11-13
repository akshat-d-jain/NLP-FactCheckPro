
***Fact Check Pro: Multi-Language and Multi-Domain Factuality Detection Using BERT-Based Similarity Analysis***

**Authors:** Shreyasee Shinde, Sneh Patel, Akshat Jain, Ojas Bodke

---

## Table of Contents
- [Overview](#overview)
- [Key Features](#key-features)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [Results](#results)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

---

## Overview
Fact Check Pro is an advanced tool designed to detect factual correctness across different languages and domains. Leveraging BERT-based embeddings, it analyzes semantic proximity between claims and supporting evidence to identify misinformation. This framework combines multiple similarity metrics to provide robust and accurate factuality judgments across various scenarios, improving the reliability of factual detection in a scalable manner.

## Key Features
- **Multi-Language Support:** Processes information in multiple languages using BERT embeddings.
- **Multi-Domain Adaptability:** Handles diverse topics with scalable accuracy.
- **Robust Similarity Analysis:** Employs multiple similarity metrics like cosine similarity, L1 and L2 norms, and the Jaccard Index.
- **Case Studies Included:** Validated with real-world data from media, policy analysis, and academic contexts.

## Dataset
This project primarily utilizes the **FEVER dataset** for fact-checking and claim verification:
- **Claims:** 185,445 human-generated claims derived from Wikipedia.
- **Evidence Sentences:** Supporting or refuting sentences from Wikipedia.
- **Labels:** Claims are categorized as "Supported," "Refuted," or "NotEnoughInfo."

### Data Structure
- **Claim ID** - Unique identifier for each claim.
- **Claim Text** - Text content of the claim.
- **Label** - "Supported," "Refuted," or "NotEnoughInfo."
- **Evidence Sets** - Sentences from Wikipedia for verification.

## Methodology
Fact Check Pro uses a multi-step approach to analyze factuality:
1. **Text Preprocessing:** Standardizes input with lowercasing, punctuation removal, etc.
2. **Embedding Generation:** Converts text to embeddings using a pre-trained BERT model.
3. **Similarity Metrics Calculation:** Computes multiple similarity measures, including:
   - Cosine Similarity
   - L1 and L2 Norms
   - Jaccard Index
4. **Threshold-Based Evaluation:** Establishes factuality using optimized similarity thresholds.
5. **Visual Analysis:** Scatter plots and similarity vs. threshold analyses for model performance evaluation.
6. **Case Studies:** Demonstrates adaptability in diverse real-world scenarios.

## Results
Fact Check Pro achieves reliable factuality detection in various domains, improving accuracy and flexibility over traditional methods. The use of diverse similarity metrics enhances the model's ability to validate information across languages and contexts, preventing misinformation in media and policy analysis.

| Metric              | Value                 |
|---------------------|-----------------------|
| Cosine Similarity   | 0.2199                |
| L1 Norm             | 1.5187                |
| L2 Norm             | 5.9458                |
| Jaccard Index       | -0.7885               |
| Pearson Correlation | 0.7798                |

## Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/FactCheckPro.git
   ```
2. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
To run Fact Check Pro, use the following command:
```bash
python fact_check_pro.py --input "path/to/claims.json" --output "path/to/results.json"
```

### Arguments
- `--input` : Path to the input file containing claims.
- `--output` : Path to save the results.

## Contributing
We welcome contributions! Please fork this repository and create a pull request for any new features, bug fixes, or improvements. Make sure your code follows the project's coding standards.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```
