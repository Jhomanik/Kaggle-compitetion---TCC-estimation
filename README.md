# Kaggle-competetion---TCC-estimation
Here is the Notebook for optimized NN training using the full potential of GPU by means of parallel data preprocessing  with multiple threads.
This scheme optimizes preprocessing of data: first of all, multiple threads preprocess batches of data independently and after safely put it to CPU queue, transfer thread removes data from CPU queue to GPU queue, and the last one transfers GPU batches to model. Thus,  all potential and power of the GPU are utilized allowing the model to train much faster.

Model is built in the PyTorch framework, more information about architecture and training cycle can be found in Notebook.

More information about competition and data itself can be found in attached file 'Competetion_info'.
