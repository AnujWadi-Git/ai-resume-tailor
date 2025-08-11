# ai-resume-tailor
AI-powered resume tailoring tool using Google Gemini - outputs Word files with optimized skills sections


# 🤖 AI Resume Tailoring Tool

An intelligent resume tailoring tool that uses **Google Gemini AI** to automatically optimize your resume's skills section based on job descriptions. Outputs properly formatted Word documents while maintaining one-page resume limits.

![Python](https://img.shields.io/badge/python-v3.7+-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![AI](https://img.shields.io/badge/AI-Google%20Gemini-orange.svg)

## ✨ Features

- 🎯 **Smart Skills Matching**: AI-powered analysis of job descriptions to tailor your skills section
- 📄 **Word Output**: Generates `.docx` files instead of PDFs for easy editing
- 🎨 **Proper Formatting**: Maintains 9pt font and bolds key technologies automatically
- 📏 **One-Page Limit**: Keeps your resume concise and recruiter-friendly
- 🔍 **ATS Optimized**: Uses keywords that pass Applicant Tracking Systems
- 💻 **Dual Interface**: Both command-line and web-based Streamlit interface
- 🆓 **Free to Use**: Uses Google Gemini's free tier

## 🚀 Quick Start

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/ai-resume-tailor.git
cd ai-resume-tailor
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

### 3. Get Google AI API Key
1. Visit [Google AI Studio](https://makersuite.google.com/app/apikey)
2. Click "Create API Key"
3. Copy your API key

### 4. Run the Tool

**Option A: Web Interface (Recommended)**
```bash
streamlit run resume_tailor.py
```
Then open your browser to the displayed URL (usually `http://localhost:8501`)

**Option B: Command Line**
```bash
python resume_tailor.py --resume your_resume.docx --job-text "paste job description here" --output tailored_resume.docx --api-key your_api_key
```

## 🖥️ Web Interface Preview

The Streamlit web interface provides:
- Easy file upload for your resume
- Text area for job description input
- Real-time preview of changes
- One-click download of tailored resume
- Skills comparison view

## 📋 Requirements

- Python 3.7 or higher
- Google AI API key (free tier available)
- Your resume in `.docx` format

## 📦 Dependencies

```
python-docx>=0.8.11
google-generativeai>=0.3.0
streamlit>=1.28.0
```

## 🛠️ How It Works

1. **Upload Resume**: Provide your base resume in Word format
2. **Job Analysis**: Paste the job description you're targeting
3. **AI Processing**: Google Gemini analyzes both documents
4. **Skills Optimization**: AI rewrites your skills section with relevant keywords
5. **Formatting**: Applies proper 9pt font and bold formatting
6. **Export**: Download your tailored resume in Word format

## 📝 Usage Examples

### Command Line Examples

**Basic usage:**
```bash
python resume_tailor.py --resume resume.docx --job-text "Software Engineer position requiring Python, React, and AWS experience..." --output tailored.docx --api-key your_key
```

**Using job description file:**
```bash
python resume_tailor.py --resume resume.docx --job-description job_desc.txt --output tailored.docx --api-key your_key
```

**Using environment variable for API key:**
```bash
export GOOGLE_API_KEY="your_api_key_here"
python resume_tailor.py --resume resume.docx --job-text "job description" --output tailored.docx
```

## 🔒 Privacy & Security

- **No Data Storage**: Your resume and job descriptions are not stored anywhere
- **Local Processing**: All file handling happens on your machine
- **API Only**: Only skills optimization requests are sent to Google Gemini
- **Open Source**: Full code transparency - review what the tool does

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Make your changes
4. Commit your changes (`git commit -m 'Add amazing feature'`)
5. Push to the branch (`git push origin feature/amazing-feature`)
6. Open a Pull Request

### Ideas for Contributions
- Add support for different resume formats
- Implement other AI models (OpenAI, Anthropic)
- Add resume templates
- Improve skills categorization
- Add job description analysis features

## 🐛 Troubleshooting

**Common Issues:**

1. **"ModuleNotFoundError"**
   ```bash
   pip install -r requirements.txt
   ```

2. **"API key not found"**
   - Make sure you have a valid Google AI API key
   - Set it as environment variable or use `--api-key` parameter

3. **"No skills section found"**
   - Ensure your resume has a clear "Skills" or "Technical Skills" section
   - The tool looks for common skills headers

4. **"Resume too long"**
   - The tool is optimized for one-page resumes
   - Consider shortening other sections if needed

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Google Gemini AI for powerful language processing
- Streamlit for the amazing web framework
- python-docx for Word document handling
- The open-source community for inspiration and tools

## 📞 Support

If you encounter any issues or have questions:
1. Check the [Issues](https://github.com/yourusername/ai-resume-tailor/issues) page
2. Create a new issue if your problem isn't already reported
3. Provide as much detail as possible for faster resolution

## 🌟 Star This Project

If this tool helps you land your dream job, please give it a star! ⭐

---

**Disclaimer**: This tool is designed to help optimize resumes but always review the AI-generated content before submitting to employers. Ensure all skills listed accurately represent your abilities.
