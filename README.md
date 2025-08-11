# Language-Guided_AudioSeparation
This project develops a system that separates audio sources from mixtures using natural language queries. By combining audio signal processing with deep learning architectures such as ResUNet and Transformer, and leveraging contrastive language-audio pretraining (CLAP), the system links textual descriptions to specific audio features. A two-phase transfer learning approach fine-tunes the pre-trained **AudioSep** model for domain-specific tasks, with a focus on separating violin and trumpet sounds.

The model demonstrates strong performance in extracting underrepresented instruments like trumpets, with improvements in Signal-to-Distortion Ratio (SDR) and spectrum consistency after fine-tuning. While violin separation remains robust from pre-training, trumpet extraction benefits significantly from targeted adaptation. The resulting system has potential applications in music production, sound editing, and assistive listening.

## TABLE I: Comparison of SDR and SDRi for Violin and Trumpet Separation
## TABLE II: Comparison of SDR and SDRi for Violin and Trumpet Separation
| Instrument | Model              | Correlation | MSE    |
|------------|--------------------|-------------|--------|
| Violin     | Pre-trained Model  | 0.9933      | 0.0006 |
| Violin     | Fine-Tuned Model   | 0.9898      | 0.0009 |
| Trumpet    | Pre-trained Model  | 0.2872      | 0.0272 |
| Trumpet    | Fine-Tuned Model   | 0.9575      | 0.0006 |

## Visualization of separation results
<img width="1693" height="764" alt="image" src="https://github.com/user-attachments/assets/28d708dc-35e1-4e56-aedb-4d4614853408" />
