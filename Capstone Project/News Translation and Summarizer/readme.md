# News Translation & Summarization with Language Detection

This Python project fetches news article from any URL, detects their language, translates into English and generates concise summaries — helping you grasp global news in seconds! <br/>
It leverages **Gradio** for the user interface, **Huggingface's transformers** for translation and summarization, **Newspaper3k** for article extraction, and **Langdetect** for language detection.

## Libraries & Teachnologies Used
- **Gradio**: For creating the user interface.
- **Huggingface Transformers**: Pre-trained models for translation and summarization.
- **Newspaper3k**: For fetching and parsing articles from URLs.
- **Langdetect**: To detect the language of the article.
- **Torch**: For managing GPU and CPU devices.

## Model Details
**Translation Models**: <br/>
`Helsinki-NLP's OPUS-MT` models for Arabic, Chinese, and Japanese translations.

**Summarization Model**: <br/> 
`Facebook's BART-Large-CNN` for summarizing the translated text.

## GPU Support
The application checks for GPU availability and will utilize it if present. If no GPU is available, the application will run on the CPU. For faster results, especially with larger texts, using Google Colab with GPU is recommended.

## NOTE
For Best Results: Run on Google Colab
To get better performance (especially with GPU), it's recommended to run this project on Google Colab. You can access GPU resources for faster translation and summarization:

- Open Google Colab.
- Upload your script or notebook to Colab.
- Ensure the runtime is set to GPU (go to Runtime -> Change runtime type -> Select GPU).
- Install the required packages by running:
- !pip install gradio !pip install transformers !pip install newspaper3k !pip install langdetect
- Execute the cells, and enjoy improved performance!
