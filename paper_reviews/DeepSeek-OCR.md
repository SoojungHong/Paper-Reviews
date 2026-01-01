## paper 
DeepSeek-OCR: Contexts Optical Compression 

## Summary 
- Compressing long contexts via optical 2D mapping

- DeepEncoder serves as the core engine, designed to maintain low activation under high-resolution input while achieving high compression ratios ensure an optimal and manageable number of vision tokens.

- Vision-text token compression ratios, achieves 96%+ OCR decoding precision at 9-10x text compression

- vision-text compression can achieve significant token reduction (7-20x) for different historical context stages, offering a promising direction for addressing long context challenges in large language models.

- The architecture of DeepSeek-OCR : consists of DeepEncoder and DeepSeek-3B-MoE decoder
- DeepEncoder is the core of DeepSeek-OCR, comprising three components : a SAM for perception dominated by window attention, a CLIP for knowledge with dense global attention, and a  16X token compressor that bridges between them

- DeepEncoder is responsible for extracting image features and tokenizing as well as compressng visual representations.

- Decoder is used for generating the required result based on image tokens and prompts 
  
## Terminology to learn 
- Low activation

- Low activation at high resolutions

- memory forgetting mechanism in LLMs

- SAM architecture

- Window attention

- CLIP architecture

- How MoE works and its architecture 

  
