# AI Apps

A collection of practical AI applications built with Google's Gemini API. These applications demonstrate the capabilities of the Gemini model for various use cases including chatbots, email generation, and text summarization.

## 📱 Applications

### 1. **AI Chatbot** (`AI_Chatbot_app.ipynb`)
A simple interactive chatbot powered by Gemini that can answer general questions and provide information.

**Features:**
- Basic conversational AI
- Instant responses to user queries
- Temperature control for response consistency
- Simple exit mechanism

**Example Usage:**
```
You: Can you list indian states
AI: India currently has 28 states and 8 union territories...
```

**Configuration:**
- Model: `gemini-3.1-flash-lite`
- Temperature: 0 (deterministic responses)

---

### 2. **Chatbot with System Prompt** (`Chatbot_with_Prompt.ipynb`)
An advanced chatbot that maintains conversation history and uses system prompts for personalized interactions.

**Features:**
- **Conversation Memory**: Maintains full conversation history for contextual responses
- **System Prompt**: Customizable system instructions to define chatbot personality
- **Personalization**: Remember user context and preferences across messages
- **Dynamic Temperature**: Set to 0.7 for more creative responses

**Example Usage:**
```
System Prompt: "My Name is Bhavani. I am from Hyderabad. I am a Software Engineer."

You: Hi
AI: Hello Bhavani! It's a pleasure to meet you...

You: Can you tell me visiting places in Hyderabad
AI: Hyderabad is a beautiful blend of rich history and modern infrastructure...
```

**Key Differences from Basic Chatbot:**
- Maintains conversation history
- Uses system instructions for personality
- More natural and contextual responses

---

### 3. **Email Generator** (`Email_Generator.ipynb`)
An AI-powered tool that generates professional emails for various scenarios.

**Features:**
- Generates multiple email options for the same request
- Professional tone and formatting
- Handles various email types (sick leave, job applications, inquiries, etc.)
- Provides tips and best practices

**Example Usage:**
```
What email do you want to write?
> Sick Leave

Output: 
- Option 1: Standard (Clear and concise)
- Option 2: With task delegation
- Option 3: Extended absence notification
```

**Email Types Supported:**
- Sick leave notifications
- Professional inquiries
- Job applications
- Business communications
- Meeting requests

---

### 4. **Text Summarizer** (`text_summarizer_app.ipynb`)
A simple text summarization tool that condenses long texts into concise summaries.

**Features:**
- Summarizes long texts efficiently
- System instruction for focused summarization
- Quick and straightforward interface

**Example Usage:**
```
Enter long text: Rubio's India itinerary, scheduled from May 23 to 26...

Summary:
Rubio's visit to India (May 23–26) is considered diplomatically significant...
```

---

## 🛠️ Prerequisites

### Required
- **Python 3.x**
- **Google Colab** (recommended for easy setup)
- **Google API Key** for Gemini API access

### Installation

1. **Get a Google API Key:**
   - Visit [Google AI Studio](https://aistudio.google.com/apikey)
   - Create a new API key
   - Store it securely

2. **In Google Colab:**
   - Add your API key to Colab Secrets:
     1. Click the "🔑 Secrets" icon in the left sidebar
     2. Create a new secret named `GOOGLE_API_KEY`
     3. Paste your API key

3. **Install Dependencies:**
   ```python
   # In Colab, these are typically pre-installed
   # If needed:
   pip install google-genai
   ```

---

## 🚀 How to Use

### Running in Google Colab

1. Open any `.ipynb` file in this repository
2. Click "Open in Colab" button (if available)
3. Add your `GOOGLE_API_KEY` to Colab Secrets
4. Run all cells (`Ctrl + F9`)

### Running Locally

```bash
# Clone the repository
git clone https://github.com/bhavani-adk/ai-apps.git
cd ai-apps

# Install dependencies
pip install google-genai

# Convert and run Jupyter notebook
jupyter notebook AI_Chatbot_app.ipynb
```

---

## 📊 Model Configuration

All applications use the **Gemini 3.1 Flash Lite** model for:
- Fast response times
- Cost efficiency
- Sufficient capability for practical tasks

### Common Parameters:

| Parameter | Value | Purpose |
|-----------|-------|---------|
| `model` | `gemini-3.1-flash-lite` | Lightweight, fast model |
| `temperature` | 0 - 0.7 | Controls response creativity (0=deterministic, 1=creative) |
| `top_p` | 0.95 | Controls diversity of responses |
| `top_k` | 20 | Limits vocabulary selection |

---

## 🎯 Use Cases

- **Personal Assistant**: Use the chatbot for quick information
- **Professional Communications**: Generate emails with the Email Generator
- **Content Management**: Summarize documents and articles
- **Learning**: Understand how to integrate Gemini API into applications

---

## 🤝 Contributing

Feel free to:
- Add new AI applications
- Improve existing applications
- Report issues
- Suggest features

---

## 📝 License

This project is open source and available under the MIT License.

---

## 📧 Contact

For questions or suggestions, feel free to reach out or open an issue in the repository.

---

## 🔗 Resources

- [Google Gemini API Documentation](https://ai.google.dev/)
- [Google Colab](https://colab.research.google.com/)
- [Gemini Python SDK](https://github.com/google/generative-ai-python)

---

**Last Updated:** May 23, 2026
