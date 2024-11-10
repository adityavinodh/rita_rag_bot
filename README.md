# RITA (RAG-Integrated Tech Assistant)

RITA is an interactive AI assistant designed to empower **senior citizens** and **visually impaired users** in navigating technology effortlessly. This project leverages state-of-the-art AI capabilities to provide hands-free, voice-activated assistance using both **speech** and **text inputs**. RITA is built on top of powerful technologies like **NVIDIA RIVA** microservices and **Meta’s Llama 3.2-3b Instruct LLM**, making it an accessible, user-friendly solution for those who may find typing challenging or unfamiliar.

## Key Features
- **Speech and Text Interaction**: Supports both voice and text commands for a personalized user experience.
- **Retrieval-Augmented Generation (RAG)**: Powered by **LlamaIndex**, RITA can fetch accurate, context-rich answers from a vast knowledge base.
- **Expanding Knowledge Repository**: Includes thousands of pages of Apple product user guides and manuals, with flexibility to add new content domains.
- **Step-by-Step Guidance**: Delivers jargon-free instructions with follow-ups for added clarity, making tech tasks manageable.
- **Safety and Guardrails**: Integrated **NeMo Guardrails** ensure conversations stay focused on tech support, avoiding sensitive topics.

Our goal is to **bridge the digital divide**, fostering digital inclusion and enhancing the quality of life for our users.

## Getting Started

### Prerequisites
- **Python 3.8+**
- **Google Colab** (for cloud execution)
- **NVIDIA RIVA** microservices (set up according to [NVIDIA documentation](https://developer.nvidia.com/riva))
- **API Keys** for access to LlamaIndex and NVIDIA services (provided in `api_keys` file)

### Installation & Setup
1. **Clone the Repository**:
    ```bash
    git clone https://github.com/yourusername/rita_rag_bot.git
    cd rita_rag_bot
    ```

2. **Upload Files to Google Drive**:
   - Download the folder and upload it to your personal Google Drive.

3. **Main Notebook**:
   - Use Google Colab to open the `app.ipynb` notebook.
  
4. **Edit Paths and API Keys**:
   - Update the paths in **Chunk 3** to point to your Google Drive location.
   - Insert your API keys from the `api_keys` file.
   - Run all cells to start the RITA bot.

5. **Enable microphone settings on browser**
    - Once all chunks are run, open the gradio interface using the link.
    - You may have to change browser preferences to allow microphones input for speech commands.
    - Enable all popups.

### Usage
- **Voice Commands**: Simply speak to RITA for hands-free interaction.
- **Text Input**: Type your queries if you prefer.
- RITA uses a **context-rich retrieval system** to provide accurate answers, especially helpful for tech support.

### Example Questions for Demo
If you're demonstrating RITA's capabilities, here are some questions you can ask:

1. **"How do I unlock my iPhone?"**
2. **"Can you show me how to adjust the screen brightness?"**
3. **"How do I make a phone call to my daughter?"**
4. **"Can you help me set a reminder?"**
5. **"How do I connect my Bluetooth hearing aids?"**

These examples highlight RITA's ability to guide users through common iPhone tasks, enhancing tech accessibility.

### Data Collection Scripts
- **iphone_16_manual_scraper.py**: Extracts content from iPhone 16 PDF manuals and saves it in JSON format.
- **emanual_scraper.py**: Extracts all links from various brands using a specified HTML pattern, converting web-based manuals to JSON.

### Future Expansion
- The current knowledge base focuses on Apple product guides but can be easily expanded to include other technology domains.
- RITA’s framework is designed to support dynamic growth, adapting to user needs as new content is added.

## Contributing
We welcome contributions! If you'd like to improve RITA, feel free to:
1. Fork the repository.
2. Create a new branch.
3. Make your changes.
4. Submit a pull request.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact
For questions or support, please reach out to **av364@cornell.edu**.

---

Thank you for using RITA to empower senior citizens and bridge the digital divide!
