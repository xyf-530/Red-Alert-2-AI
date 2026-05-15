# Red-Alert-2-AI
AI for Red Alert 2
Based on Qwen3.5, the visual head is used as high-definition input, and the compressed image through multiple layers of {Pixel-Shuffle + MLP} is used as the input of the LLM backbone. Multiple cross-attentions are added to enable mutual injection between the visual and historical aspects. Parallel sequence prediction is planed to be implemented as training strategy. The pre-training dataset contains only two to three hundred games, and PPO is planned to be used for subsequent training.
Currently, we don't know why KV Cache is not working properly, so we are planning to bypass it.
