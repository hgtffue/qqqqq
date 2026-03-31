CIFAR-100 clusters=100

| | Prompt | Noise ratio | $H(Y \mid \bar{Y})$ | $I(Y; \bar{Y})$ | FWD | CPE |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Qwen3-VL-8B | Current prompt | 0.07% | 5.5897 | 1.0542 | 36.92±0.45 | 36.77±0.40 |
| LLaVA-7B | Current prompt | 0.23% | 4.5727  | 2.0711 | 46.70±0.60 | 46.57±0.09 |

| | Prompt | Noise ratio | $H(Y \mid \bar{Y})$ | $I(Y; \bar{Y})$ | FWD | CPE |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| LLaVA-7B | Current prompt | 0.23% | 4.5727  | 2.0711 | 46.70±0.60 | 46.57±0.09 |
| LLaVA-7B | New prompt | 0.14% | 5.5897 | 1.0397 | 36.83±0.71 | 36.49±0.68 |

**Current prompt:**
`"[INST] <image>\n Which label does not belong to this image? Answer the question with a single word: {label[0], label[1], label[2], label[3]} [/INST]"`

**New negative prompt:**
`"[INST] <image>\n Which label does not belong to this image? (1) {labels[0]} (2) {labels[1]} (3) {labels[2]} (4) {labels[3]} Please respond with only the number of the correct answer [/INST]"`