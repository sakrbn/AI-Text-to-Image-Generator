# AI Text-to-Image Generator

A powerful and user-friendly application for generating images from text descriptions using Stable Diffusion models. This project includes two versions: a simple implementation for beginners and an advanced version with professional features.

## 🌟 Features Overview

### Simple Version (Recommended for Beginners)
- **4 AI Models**: SD 1.5 Fast, SD 1.5 Quality, SDXL Base, OpenJourney
- **Easy-to-use Interface**: Clean and intuitive Gradio web interface
- **Multiple Image Sizes**: Square, landscape, portrait, and wide formats
- **Generation History**: Track and review your previous generations
- **Smart Model Management**: Automatic memory optimization
- **Generation Limits**: 500 images per session
- **Progress Tracking**: Real-time generation progress with visual feedback

### Advanced Version (Professional Features)
- **6 AI Models**: Including specialized models like DreamShaper and Realistic Vision
- **8 Style Presets**: Photorealistic, Digital Art, Anime, Fantasy, Cyberpunk, Oil Painting, Watercolor, 3D Render
- **Post-Processing**: Real-time brightness, contrast, saturation, and sharpness adjustments
- **Batch Generation**: Generate multiple variations at once
- **Analytics Dashboard**: Interactive charts showing usage statistics and trends
- **Preset Management**: Save and load your favorite settings
- **Template Builder**: Quick prompt generation with predefined templates
- **Favorites System**: Bookmark your best generations
- **Export Functionality**: Export history in JSON or CSV format
- **Enhanced UI**: Modern animated interface with advanced styling
- **Generation Limits**: 1000 images per session

## 🚀 Quick Start

### Requirements
- Python 3.8+
- CUDA-compatible GPU (recommended) or CPU
- 8GB+ RAM (16GB+ recommended for SDXL models)

### Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/ai-image-generator.git
cd ai-image-generator

# Install dependencies (automatically handled by the scripts)
# The scripts will install: gradio, diffusers, transformers, accelerate, safetensors
```

### Running the Simple Version

```python
# Copy and run the simple version code
python simple_generator.py
```

### Running the Advanced Version

```python
# Copy and run the advanced version code  
python advanced_generator.py
```

## 📋 Usage Guide

### Step-by-Step Instructions

1. **Launch the Application**
   - Run the Python script
   - Open the provided URL in your browser
   - The interface will load automatically

2. **Select and Load a Model**
   - Choose from available AI models
   - Click "Load Model" and wait for confirmation
   - Model loading may take 1-5 minutes depending on your internet speed

3. **Create Your Prompt**
   - Write a detailed description of your desired image
   - Use English for best results
   - Include style keywords like "highly detailed", "8k", "professional"

4. **Configure Settings**
   - **CFG Scale**: Controls prompt adherence (7-10 recommended)
   - **Steps**: Generation quality (30-50 for good balance)
   - **Image Size**: Choose based on your model and needs
   - **Seed**: Use same seed to reproduce results (-1 for random)

5. **Generate Images**
   - Click "Generate" and wait for results
   - Generation time varies from 30 seconds to 5 minutes

## 🤖 Model Comparison

| Model | Speed | Quality | Memory Usage | Best For |
|-------|--------|---------|--------------|----------|
| SD 1.5 Fast | ⚡⚡⚡⚡⚡ | ⭐⭐⭐ | Low | Quick iterations, testing |
| SD 1.5 Quality | ⚡⚡⚡ | ⭐⭐⭐⭐ | Medium | Balanced performance |
| SDXL Base | ⚡⚡ | ⭐⭐⭐⭐⭐ | High | Maximum quality, final results |
| OpenJourney | ⚡⚡⚡⚡ | ⭐⭐⭐⭐ | Medium | Artistic styles |
| DreamShaper | ⚡⚡⚡ | ⭐⭐⭐⭐ | Medium | Fantasy, surreal images |
| Realistic Vision | ⚡⚡⭐ | ⭐⭐⭐⭐⭐ | Medium | Photorealistic portraits |

## 🎨 Style Presets (Advanced Version)

- **Photorealistic**: Ultra-realistic photos with professional quality
- **Digital Art**: Modern digital illustrations and concept art
- **Anime**: Japanese animation style with vibrant colors
- **Fantasy**: Magical and ethereal artwork
- **Cyberpunk**: Futuristic neon aesthetics and tech noir
- **Oil Painting**: Traditional art with visible brushstrokes
- **Watercolor**: Soft edges and artistic traditional media
- **3D Render**: High-quality 3D rendered appearances

## 💡 Pro Tips

### Prompt Engineering
- Be specific and descriptive
- Include quality keywords: "masterpiece", "best quality", "highly detailed"
- Mention art styles: "digital painting", "photorealistic", "concept art"
- Add technical terms: "8k uhd", "professional photography", "cinematic lighting"

### Parameter Optimization
- **CFG Scale**: 1-5 (very creative), 7-10 (balanced), 15+ (strict prompt following)
- **Steps**: 20-30 (fast), 30-50 (quality), 50+ (maximum quality)
- **Negative Prompts**: Use to avoid unwanted elements

### Performance Tips
- Start with SD 1.5 models for testing
- Use lower steps for experimentation
- Switch to SDXL for final high-quality results
- Enable memory optimizations for large images
- Use batch generation for variations

## 🔧 Troubleshooting

### Common Issues

**Out of Memory Errors**
- Reduce image size
- Use SD 1.5 instead of SDXL
- Enable CPU offload
- Restart the application

**Slow Generation**
- Lower the number of steps
- Use faster models (SD 1.5 Fast)
- Reduce image size
- Check GPU availability

**Poor Quality Results**
- Increase steps (30-50)
- Adjust CFG scale (7-10)
- Improve prompt description
- Use negative prompts
- Try different models

**Model Loading Failures**
- Check internet connection
- Restart the application
- Clear browser cache
- Verify GPU memory availability

## 📊 Technical Specifications

### System Requirements
- **Minimum**: 8GB RAM, modern CPU, 10GB storage
- **Recommended**: 16GB+ RAM, CUDA GPU with 8GB+ VRAM, 20GB storage
- **Optimal**: 32GB RAM, RTX 3080/4080 or better, SSD storage

### Supported Formats
- **Output**: PNG (high quality, no compression)
- **Resolutions**: 512x512 to 1536x640 (depending on model)
- **Export**: JSON and CSV for generation history

## 🤝 Contributing

Contributions are welcome! Please feel free to submit pull requests or open issues for:
- Bug fixes and improvements
- New model integrations
- UI/UX enhancements
- Performance optimizations
- Documentation updates

## 📄 License

This project is open source. Please check the license file for details.

## 🙏 Acknowledgments

- Stability AI for Stable Diffusion models
- Hugging Face for model hosting and diffusers library
- Gradio team for the amazing web interface framework
- The open-source AI community for continuous improvements

## 📞 Support

If you encounter any issues or have questions:
1. Check the troubleshooting section above
2. Review existing GitHub issues
3. Create a new issue with detailed information
4. Include system specifications and error messages

---

**Note**: This application is designed for creative and educational purposes. Please use responsibly and respect content policies when generating images.

## 🚀 Getting Started Examples

### Basic Prompt Examples
```
"A beautiful sunset over mountains, landscape photography, golden hour"
"Portrait of a wise old wizard, fantasy art, detailed"
"Modern city skyline at night, cyberpunk style, neon lights" 
"Cute cat sleeping in a garden, soft lighting, peaceful"
```

### Advanced Prompt Examples
```
"Epic dragon soaring over ancient castle, fantasy concept art, dramatic lighting, highly detailed, 8k resolution, trending on artstation"
"Professional headshot of businesswoman, corporate photography, studio lighting, sharp focus, photorealistic, 85mm lens"
"Steampunk mechanical owl with brass gears, Victorian era aesthetic, intricate details, warm golden lighting, digital art masterpiece"
```

Happy generating! 🎨✨
