# RAG Pipeline with Retrieval Evaluation

- This week's assignment builds and evaluates an end-to-end retrieval-augmented generation (RAG) 
system over an eight-document corpus about RAG concepts. 
It compares three chunk configuration settings for recall and precision at the top-5 chunk level.

# Chunk setting

- Three chunk configurations were chosen with a fixed word configuration
80/20, 160/40, 320/80 for chunk size/overlap.

# Produced chunks, recall, and precision.

==> Each configuration produced 16, 8, and 8 chunks, respectively.

==> All three settings achieved a mean of 1.00 @5.

==> 80/20 achieved a mean precision of 0.22 @5.

==> 160/40 and 320/80 achieved a mean precision of 0.2 @5.
