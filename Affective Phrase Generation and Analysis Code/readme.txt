==== Affective Phrase Set Generation and Analysis ====

We provide Python code to allow you to create your own affective phrase sets and select the best ones to use for transcription tasks. 

For this, you will need to setup an LLM server (we use LMStudio) with an LLM of your own choice (we used Llama3.1-8b). Additionally, you will need to download the VA classifier model by Mendes & Martins, see their paper here: https://doi.org/10.1007/978-3-031-28244-7_6 and code repository here: https://github.com/gmendes9/multilingual_va_prediction