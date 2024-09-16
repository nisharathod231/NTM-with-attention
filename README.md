# NTM-with-attention
This project explores the use of attention mechanisms to translate human-readable dates into machine-readable formats. The task is inspired by the works of Bahdanau et al. (2014) and Luong et al. (2015), focusing on neural machine translation (NMT) with attention.

![image](https://github.com/user-attachments/assets/3b29f524-1ca8-4eb6-b340-18eec0b5fc9b)

## Dataset

- **Training Set**: `Datasets/train.txt` (36,000 examples)
- **Validation Set**: `Datasets/validation.txt`
- Each example in the dataset consists of a human-readable date (e.g., "Saturday 29 February 2021") and the corresponding machine-readable format (e.g., "2021-02-29").

## Task

Translate dates such as:
- "Saturday 29 February 2021" to "2021-02-29"
- "29 February 2020" to "2020-02-29"
- "Fri 1867 15 november" to "1867-11-15"

Additionally, visualize the parts of the input to which each output attends while doing the translation using the trained model.

## Models and Methods

### Attention Mechanisms:
- **Bahdanau Attention**: [Bahdanau et al., 2014](https://arxiv.org/pdf/1409.0473.pdf)
- **Luong Attention**: [Luong et al., 2015](https://arxiv.org/pdf/1508.04025.pdf)

We employ the attention mechanisms described in these papers to enhance the performance of the sequence-to-sequence model in translating dates.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/date-translation-attention.git
    cd date-translation-attention
    ```
    
2. Run train.ipnyb to get model.pth

3. Run the test.ipynb to get predictions.xslx

## Results

Results are reported on the validation set using the trained model. For the given examples:

********************Epoch 10********************
- Train Loss: 0.062
- Validation Loss: 0.065


### Attention Visualization
The model visualizes which parts of the input sequence the output sequence attends to during translation.

![image](https://github.com/user-attachments/assets/47f46ef3-7eb7-460b-ab0c-a23cfa1c3409)


## References

1. **Bahdanau et al., 2014** - [Neural Machine Translation by Jointly Learning to Align and Translate](https://arxiv.org/pdf/1409.0473.pdf)
2. **Luong et al., 2015** - [Effective Approaches to Attention-Based Neural Machine Translation](https://arxiv.org/pdf/1508.04025.pdf)
