# Blog Images Generator

A Node.js tool that generates beautiful abstract background images for blog posts using OpenAI's DALL-E image generation API. This project creates 100 unique abstract backgrounds with soft-focus gradients in various color combinations, perfect for blog post cover images.

## Features

- 🎨 **100 Unique Designs**: Pre-defined prompts for diverse color combinations
- 📐 **Multiple Sizes**: Generates images in 1536x1024 and 384x256 resolutions
- 🌈 **Color Variety**: From pastel blues and purples to warm ambers and corals
- 🎯 **Blog-Optimized**: Designed specifically for blog post cover images
- ⚡ **Fast Generation**: Uses OpenAI's latest image generation model

## Images

<table>
  <tr>
    <td><img src="https://raw.githubusercontent.com/AnandChowdhary/blog-images/refs/heads/main/384x256/1.png"></td>
    <td><img src="https://raw.githubusercontent.com/AnandChowdhary/blog-images/refs/heads/main/384x256/2.png"></td>
    <td><img src="https://raw.githubusercontent.com/AnandChowdhary/blog-images/refs/heads/main/384x256/3.png"></td>
    <td><img src="https://raw.githubusercontent.com/AnandChowdhary/blog-images/refs/heads/main/384x256/4.png"></td>
    <td><img src="https://raw.githubusercontent.com/AnandChowdhary/blog-images/refs/heads/main/384x256/5.png"></td>
  </tr>
</table>

## Prerequisites

- Node.js (v16 or higher)
- OpenAI API key

## Installation

1. Clone the repository:

```bash
git clone https://github.com/AnandChowdhary/blog-images.git
cd blog-images
```

2. Install dependencies:

```bash
npm install
```

3. Set up your OpenAI API key:

```bash
export OPENAI_API_KEY="your-api-key-here"
```

## Usage

Run the image generation script:

```bash
node generate.mjs
```

This will:

- Generate 100 unique abstract background images
- Save them in the `1536x1024/` directory
- Use the predefined prompts for consistent, blog-friendly designs

## Generated Images

The script creates abstract backgrounds with:

- **Soft-focus effects** for a dreamy, professional look
- **Smooth gradients** for visual appeal
- **Minimal texture** to avoid distraction from text
- **Pastel and vibrant color combinations** for variety

### Sample Color Combinations

- Pastel blues and purples
- Sunset orange and pink
- Cool greens and aquamarine
- Gold and rose pink
- Coral and mint
- And 95+ more unique combinations

## File Structure

```
blog-images/
├── 1536x1024/          # High-resolution images (1536x1024)
├── 384x256/            # Thumbnail images (384x256)
├── generate.mjs        # Main generation script
├── package.json        # Project dependencies
└── README.md          # This file
```

## Configuration

The generation script uses:

- **Model**: `gpt-image-1` (OpenAI's latest image generation model)
- **Quality**: `low` (for faster generation and cost efficiency)
- **Size**: `1536x1024` (optimal for blog covers)

## Cost Considerations

- Each image generation costs approximately $0.02-0.04 USD
- Generating all 100 images costs approximately $2-4 USD
- The script uses "low" quality setting to minimize costs

## Customization

To modify the generated images:

1. Edit the `prompts` array in `generate.mjs`
2. Change the `size` parameter for different dimensions
3. Adjust the `quality` setting (standard/hd) for different quality levels
