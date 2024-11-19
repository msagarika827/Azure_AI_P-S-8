
# Speaking Clock Application

This project is a simple Speaking Clock app that uses the Azure AI Speech service. It utilizes both Speech-to-Text and Text-to-Speech APIs to recognize spoken commands and respond with audible speech. The application is developed in  Python, and it can tell you the current time based on your spoken query.

## Table of Contents

- [Overview]
- [Prerequisite]
- [Setup]
- [Running the Application]
- [Usage]
- [Customization]
- [Troubleshooting]
- [References]

## Overview

The Speaking Clock application uses Azure AI Speech SDK to:
- Convert spoken input (e.g., "What time is it?") into text.
- Synthesize speech from text to provide an audible response.

## Prerequisites

Before you begin, ensure you have the following:

- An Azure account.
- An Azure AI Speech resource (with keys and endpoint info).
- A computer with Visual Studio Code installed.
- .NET SDK installed for Python 3.x for the Python version.
- A microphone or audio file (`time.wav`) for speech input.

## Setup

### 1. Provision an Azure AI Speech Resource

1. Sign in to [Azure Portal](https://portal.azure.com/).
2. Search for **Azure AI Services** and select **Speech**.
3. Create a new Speech resource with the following settings:
   - **Subscription**:
   - **Resource group**: 
   - **Region**: 
   - **Name**: 
   - **Pricing tier**: 
   - Agree to the Responsible AI Notice.
4. Review and create the resource.
5. Go to the resource and copy the **Keys** and **Region** for later use.

### 2. Clone the GitHub Repository

1. Open Visual Studio Code.
2. Open the command palette (Ctrl+Shift+P) and run:
   ```
   Git: Clone
   ```
3. Clone the following repository:
   ```
   https://github.com/MicrosoftLearning/mslearn-ai-language
   ```
4. Open the cloned folder in Visual Studio Code.

### 3. Configure the Application
   **Python**:
   ```bash
   pip install azure-cognitiveservices-speech==1.30.0
   ```

5. Update the configuration file with your Azure AI Speech keys:
   - Python: `.env`

   Add your **region** and **key** information.

## Running the Application
### For Python:

1. Open an integrated terminal folder.
2. Run the  command:

## Troubleshooting

- If speech recognition fails, check that the **key** and **region** in the configuration file are correct.
- Ensure the Azure AI Speech SDK is installed correctly.
- If using a microphone, verify it's connected and properly configured.

## References

- [Azure AI Speech Documentation](https://learn.microsoft.com/en-us/azure/ai-services/speech-service/)
- [Voice Gallery for Azure AI Speech](https://speech.microsoft.com/portal/voicegallery)
- [Microsoft Learning GitHub Repository](https://github.com/MicrosoftLearning/mslearn-ai-language)
