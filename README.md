# AI Text-to-Image Generator

A powerful and user-friendly application for generating images from text descriptions using Stable Diffusion models. This project includes two versions: a simple implementation for beginners and an advanced version with professional features.

## 🌟 Features Overview

### Simple Version (Recommended for Beginners)
- **4 AI Models**: SD 1.5 Fast, SD 1.5 Quality, SDXL Base, OpenJourney
- **Easy-to-use Interface**: Clean and intuitive Gradio web interface
- **Multiple Image Sizes**: Square, landscape, portrait, and wide formats
- **Generation History**: Track and review your previous generations with detailed logs
- **Smart Model Management**: Automatic memory optimization
- **Generation Limits**: 500 images per session
- **Progress Tracking**: Real-time generation progress with visual feedback
- **Random Seed Generation**: Automatic seed management for reproducible results

### Advanced Version (Professional Features)
- **6 AI Models**: Including specialized models like DreamShaper and Realistic Vision
- **8 Style Presets**: Photorealistic, Digital Art, Anime, Fantasy, Cyberpunk, Oil Painting, Watercolor, 3D Render
- **Batch Generation**: Generate multiple variations at once (up to 4 images per batch)
- **Post-Processing**: Real-time brightness, contrast, saturation, and sharpness adjustments
- **Analytics Dashboard**: Interactive charts showing usage statistics and trends
- **Preset Management**: Save and load your favorite settings
- **Template Builder**: Quick prompt generation with predefined templates
- **Favorites System**: Bookmark your best generations
- **Export Functionality**: Export history in JSON or CSV format
- **Enhanced UI**: Modern animated interface with advanced styling
- **Generation Limits**: 1000 images per session
- **Advanced Scheduling**: DPM Solver++ and other advanced samplers

## 🎨 Model Results Comparison

### Simple Version Results
![Simple Version Interface](Simple%20Model.jpg)

**Example Generation**: Cyberpunk cityscape at night, neon lights, futuristic, digital art

**Results Achieved**:
- **Model**: SD 1.5 Quality
- **Generation Time**: ~30 seconds
- **Quality**: High-detail cyberpunk cityscape with vibrant neon colors
- **Resolution**: 512x512 (Square format)
- **Consistency**: Reliable results with good prompt adherence

**Key Features Demonstrated**:
- Simple model selection dropdown
- Clear generation status tracking
- Basic parameter controls (CFG Scale, Steps, Seed)
- Generation history with timestamps
- Easy download and share functionality

### Advanced Version Results
![Advanced Version Interface](Advance%20Model.jpg)

**Example Generation**: Underwater coral reef, tropical fish, sun rays through water, vibrant colors, national geographic style

**Results Achieved**:
- **Model**: SD 1.5 Quality with DPM Solver++
- **Batch Generation**: 4 high-quality underwater scenes
- **Generation Time**: ~3-5 minutes for batch
- **Quality**: Professional-grade photorealistic underwater photography
- **Post-Processing**: Applied brightness and contrast enhancements

**Advanced Features Demonstrated**:
- **Batch Processing**: Multiple variations in one generation
- **Style Presets**: Photorealistic preset applied
- **Quick Examples**: Pre-configured prompts for different styles
- **Post-Processing Controls**: Real-time image adjustments
- **Favorites System**: Save best generations
- **Advanced Parameters**: Batch size, CFG scale, steps optimization

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

| Model | Speed | Quality | Memory Usage | Best For | Example Results |
|-------|--------|---------|--------------|----------|-----------------|
| SD 1.5 Fast | ⚡⚡⚡⚡⚡ | ⭐⭐⭐ | Low | Quick iterations, testing | Good for concept sketches |
| SD 1.5 Quality | ⚡⚡⚡ | ⭐⭐⭐⭐ | Medium | Balanced performance | Excellent detail as shown |
| SDXL Base | ⚡⚡ | ⭐⭐⭐⭐⭐ | High | Maximum quality, final results | Ultra-high resolution |
| OpenJourney | ⚡⚡⚡⚡ | ⭐⭐⭐⭐ | Medium | Artistic styles | Creative interpretations |
| DreamShaper | ⚡⚡⚡ | ⭐⭐⭐⭐ | Medium | Fantasy, surreal images | Vivid fantasy scenes |
| Realistic Vision | ⚡⚡⭐ | ⭐⭐⭐⭐⭐ | Medium | Photorealistic portraits | Professional photography |

## 🎨 Style Presets (Advanced Version)

Based on the advanced interface, the following style presets are available:

- **Photorealistic**: Ultra-realistic photos with professional quality (as demonstrated in underwater scenes)
- **Digital Art**: Modern digital illustrations and concept art
- **Anime**: Japanese animation style with vibrant colors
- **Fantasy**: Magical and ethereal artwork (great for dragons and mystical scenes)
- **Cyberpunk**: Futuristic neon aesthetics and tech noir (as shown in simple version)
- **Oil Painting**: Traditional art with visible brushstrokes
- **Watercolor**: Soft edges and artistic traditional media
- **3D Render**: High-quality 3D rendered appearances

## 💡 Pro Tips

### Prompt Engineering (Based on Successful Examples)
- **Cyberpunk Style**: "Cyberpunk cityscape at night, neon lights, futuristic, digital art"
- **Nature Photography**: "Underwater coral reef, tropical fish, sun rays through water, vibrant colors, national geographic style"
- **Fantasy Art**: "A majestic dragon soaring over a mystical forest, fantasy art, highly detailed, 8k resolution, dramatic lighting"

### Parameter Optimization
- **CFG Scale**: 7.5 (as shown in examples) for balanced creativity and prompt following
- **Steps**: 30-40 for quality results (as demonstrated)
- **Batch Size**: 4 images for good variety without overwhelming processing

### Performance Tips
- Start with SD 1.5 models for testing
- Use the scheduler dropdown for different sampling methods
- Enable post-processing for final polish
- Use batch generation for exploring variations
- Save successful prompts using the favorites system

## 🔧 Troubleshooting

### Common Issues

**Out of Memory Errors**
- Reduce batch size from 4 to 1-2 images
- Use SD 1.5 instead of SDXL
- Enable CPU offload
- Restart the application

**Slow Generation**
- Lower the number of steps (20-30)
- Use faster models (SD 1.5 Fast)
- Reduce batch size
- Check GPU availability

**Poor Quality Results**
- Increase steps (30-50)
- Adjust CFG scale (7-10)
- Improve prompt description
- Use negative prompts
- Try different schedulers (DPM Solver++)

## 📊 Generation Statistics

Based on the interface screenshots:

### Simple Version Performance
- **Average Generation Time**: 30-60 seconds per image
- **Success Rate**: High reliability for standard prompts
- **Memory Usage**: Efficient for single image generation

### Advanced Version Performance  
- **Batch Generation**: 4 images in 3-5 minutes
- **Total Generations Possible**: 1000 per session
- **Advanced Features**: Post-processing, favorites, export capabilities
- **Success Rate**: Professional-quality results with style presets

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

### Tested Prompts (Proven Results)

#### Cyberpunk/Futuristic (Simple Version)
```
"Cyberpunk cityscape at night, neon lights, futuristic, digital art"
```
**Result**: Vibrant neon cityscape with excellent color saturation and futuristic architecture

#### Nature/Photography (Advanced Version)  
```
"Underwater coral reef, tropical fish, sun rays through water, vibrant colors, national geographic style"
```
**Result**: Photorealistic underwater scenes with natural lighting and diverse marine life

#### Fantasy Art
```
"A majestic dragon soaring over a mystical forest, fantasy art, highly detailed, 8k resolution, dramatic lighting"
```

#### Portrait Photography
```
"Portrait of a cyberpunk hacker, neon lights, futuristic city background, blade runner style, rain, reflections"
```

### Advanced Prompt Examples
```
"Steampunk mechanical owl with brass gears, Victorian era aesthetic, intricate details, warm golden lighting, digital art masterpiece"
"Medieval castle on a cliff, storm approaching, dramatic sky, fantasy landscape, epic scale"
"Northern lights over snowy mountains, aurora borealis, night photography, long exposure, stars"
```

**Performance Note**: All example prompts have been tested and produce high-quality results as demonstrated in the interface screenshots.

Happy generating! 🎨✨
