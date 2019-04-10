### Table of Contents

1. [Speech Cognitive Services](https://github.com/LaloCo/EduardoRosas/new/master#using-speech-services-for-translation)

# Using Speech Services for Translation

Recently Microsoft discontinued its Azure Speech Translate Cognitive Service, or rhater, migrated it over to
another service: the _Speech Service_. My students over on my
[Azure Cognitive Services course](https://www.udemy.com/azure-machine-learning-using-cognitive-services) were
wondering what had happened, so I created this example for them, in which they can create a recognizer using
the new SDK:

```python
recognizer = tl.TranslationRecognizer(translation_config=speech_config)
```

And then use it to translate between different languages:

```python
print("Say something in English to be translated into Spanish and German:")

result = recognizer.recognize_once()
```

[**Visit the repository here for more**](https://github.com/LaloCo/SpeechCognitiveService_Translate)
