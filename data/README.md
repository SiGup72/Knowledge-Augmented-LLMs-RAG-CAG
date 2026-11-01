# Dataset Documentation

## Dataset
**CK-12 Textbook Question Answering (TQA)**

- Hugging Face: https://huggingface.co/datasets/notefill/ck12-tqa-instruction
- Original dataset: https://prior.allenai.org/projects/tqa

## Dataset Preparation

Only text-based questions were retained. Questions requiring diagrams were excluded.

Records with inconsistent answer labels were removed. No answers were guessed or manually corrected.

## Final Dataset Statistics

| Split | Original Text-only | Cleaned | Excluded |
|---|---:|---:|---:|
| Training | 8,653 | 8,643 | 10 |
| Validation | 2,528 | 2,524 | 4 |
| Test | 2,512 | 2,508 | 4 |
| **Total** | **13,693** | **13,675** | **18** |

## Data Integrity

The cleaned dataset passed checks for:
- Duplicate IDs
- Missing IDs, questions and answers
- Answer-label mismatches
- Overlapping question IDs between splits
- Overlapping lesson IDs between splits

All checks returned zero issues.

## Knowledge Corpus

The training split was used to construct a knowledge corpus containing:
- Lesson name
- Question
- Answer options
- Correct answer

The corpus contains 8,643 entries.

It is a question-answer-derived knowledge corpus, not a collection of complete textbook lesson passages.

## Token Statistics

Tokenizer: Qwen/Qwen2.5-7B-Instruct

| Metric | Value |
|---|---:|
| Total tokens | 434,663 |
| Average tokens per entry | 50.29 |
| Median tokens per entry | 48 |
| 95th percentile | 81 |
| Maximum tokens per entry | 175 |

## License Note

The original CK-12 TQA dataset and its Hugging Face reformat may have different licensing terms. Verify the applicable license before redistributing dataset contents.

The actual dataset files are maintained separately in Google Drive and are not included in this GitHub repository.