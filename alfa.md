We started the Alpha Data Intelligence with Visual Language Model efforts in Q3. In this design, we covered a report on the current landscape for VRM with recommendations on what to build for intelligent data selection and curation for perception.

After evaluating a list of state-of-the-art models, we decided to build the framework with Qwen VL and Nvidia Cosmos Embed model

First, in collaboration with the Scalable ML team, we productionized the 2 alpha for text-to-video and video-to-video search on the entire M1 data which is 150K slices.
Embedding model itself has the fundamental limitations of information loss coming from contrastive training. We choose to use NVIDIA Cosmos Embedding model because this model has been fine-tuned with lots of emboddied AI and driving datasets. Traditionally, a clip style model wouldn't understand what is the vehicle turning right. Such simple behavior but we have seen pretty decent performance using the Nvidia Cosmos model.