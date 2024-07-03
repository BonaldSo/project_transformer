IMPLEMENTATION OF TRANSFORMER

specifications: it is built in using a MultiHeadAttention class, a FeedForward class, an EncoderBlock class, an DecoderBlock class,
a PositionEncoding class. Then they are all combined together to create a Transformer class.

usage: it takes the default numbers of src_vocab_size, tgt_vocab_size, d_embedding, n_heads, num_layers, d_ff, max_seq_length and dropout
to create the transformer. It then takes random src_data and tgt_data as input, and run with CrossEntropyLoss function and Adam optimizer.

result: we can see from the plot at the end that the training loss is decreasing after each epoch, meaning that it is learning to 
output the correct target data given the source data as input step by step. 
