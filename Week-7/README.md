# Week 7 — The Adaptation Decision and a Production Dataset**  
Focus: healthcare administrative intent classification, dynamic few-shot retrieval, and evidence-based LLM adaptation.

## Limitations

- Synthetic, template-generated requests may be less diverse than real administrative messages.
- The evaluation split is relatively small, and results may vary across API runs.
- Similar templates can appear across the train/evaluation split even when exact text overlap is prevented.
- Semantic similarity does not guarantee that the retrieved examples represent all intent classes.
- API availability, model identifiers, safety settings, and model responses can change.
- This is an experimental classifier; it is not integrated with clinical systems, patient records, appointment scheduling, or prescription services.

## Future Improvements

- Evaluate on a larger, independently labeled, privacy-preserving dataset of real-world administrative requests.
- Add template-family or paraphrase-group splits to test generalization beyond synthetic patterns.
- Compare different values of `TOP_K`, retrieval diversity, and class-balanced example selection.
- Analyze confusion patterns and malformed outputs in addition to per-intent accuracy.
- Add cost, latency, reproducibility, and uncertainty measurements.
- Reassess fine-tuning only after establishing stronger evaluation baselines.

## Technologies

- Python, Jupyter Notebook / Google Colab
- pandas, NumPy, scikit-learn
- Sentence Transformers (`all-MiniLM-L6-v2`)
- FAISS (`faiss-cpu`)
- Google GenAI SDK (`google-genai`)
- `tiktoken`
