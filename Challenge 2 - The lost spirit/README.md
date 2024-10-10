# 🎆 Challenge Two: The Lost Spirit

**Task 2.1** - Basic Sentiment Detection
**Task 2.2** - Emotion-Based Content Recommendation

## Overview

Develop an Emotional Response AI for Human-Machine Interaction

The primary objective is to create an AI system capable of understanding human emotions and suggesting appropriate content to users based on those emotions. 

## Knowledge

- Python

## Files provided

- template.py: template file you should use to write your program
- test.py: useful file to test your solution

## Dependencies & Tools

- `transformers` from `pipeline` library

## Documentation

**Goal**: Create an AI system that detects user emotions (e.g., sadness, joy) from real-time data and generates responses or media (e.g., memes, music) to improve mental well-being.
**Objective**: Focus on human-machine emotional interaction, combining AI with mental health solutions.

### Task 2.1: Basic Sentiment Detection

**Objective:** Develop a basic Natural Language Processing (NLP) model to detect user emotions from text.
**Implementation Details:** Use open-source libraries to analyze the emotional sentiment from user input (e.g., joy, sadness, anger).
**Input:** A string of text (e.g., a chat conversation).
**Output:** A basic sentiment score or classification (e.g., positive, negative, neutral).
**Resources:** Pre-trained sentiment analysis models like `DistilBERT-based Emotion classifier` from Hugging Face.

#### Test 2.1 Test Data

```python
test_data = [
    {"text": "I'm so happy with my new job!", "expected": "Joy"},
    {"text": "This is such a disappointing situation.", "expected": "Sadness"},
    {"text": "I'm scared about the upcoming exams.", "expected": "Fear"},
    {"text": "Feeling angry about the unfair treatment.", "expected": "Anger"},
    {"text": "It is shocking to see such an incident!", "expected": "Surprise"}
]
```

### Task 2.2: Emotion-Based Content Recommendation

**Objective:** Based on detected emotions from Task 2.1, generate personalized responses such as memes or quotes.
**Implementation Details:**

- Create a simple database of pre-tagged content (e.g., memes, motivational quotes) based on emotions (e.g., happy = funny meme, sad = motivational quote).
- Implement logic that matches the detected emotion to an appropriate piece of content.
- Resources: Use Python to query a small dataset or manually created content bank.

#### Test 2.2: Example content

```python
content_db = {
    "joy": ["Celebrate your wins!", "Joyful meme: https://example.com/meme1"],
    "sadness": ["You are not alone!", "Comforting meme: https://example.com/meme2"],
    "fear": ["You are stronger than you think!", "Reassuring meme: https://example.com/meme3"],
    "anger": ["Take a deep breath.", "Calming meme: https://example.com/meme4"],
    "disgust": ["Look at things with a fresh perspective.", "Positive meme: https://example.com/meme5"],
    "surprise": ["Life's full of surprises!", "Surprising meme: https://example.com/meme6"],
    "neutral": ["Stay productive!", "Calm meme: https://example.com/meme7"]
}
```

#### Test 2.2: Expected Result

```markdown
Input: "I got a promotion today!"
Emotion Detected: joy
Recommended Content: "Celebrate your wins!" 
OR
Recommended Content: "Joyful meme: https://example.com/meme1"

---

Input: "I lost my wallet and feel terrible."
Emotion Detected: sadness
Recommended Content: "You are not alone!"
OR
Recommended Content: "Comforting meme: https://example.com/meme2"

---

Input: "I have to give a big presentation tomorrow, and I'm really nervous."
Emotion Detected: fear
Recommended Content: "You are stronger than you think!"
OR
Recommended Content: "Reassuring meme: https://example.com/meme3"

---

Input: "Why was I treated so unfairly?"
Emotion Detected: anger
Recommended Content: "Take a deep breath."
OR
Recommended Content: "Calming meme: https://example.com/meme4"

---

Input: "I just found out I won a prize!"
Emotion Detected: surprise
Recommended Content: "Life's full of surprises!"
OR
Recommended Content: "Surprising meme: https://example.com/meme6"
```

## Evaluation Criteria

The submission time will not award any points; it will only be considered in the event of ties. The team with the earlier submission will be ranked above the others.

**Important Remark**: your program will be tested considering a wide range of possibilities: do not base you solution only on the example. Programs not passing 100% of tests will be penalized.

### 1. Emotion Detection Accuracy (25%)

The model should be able to provide an accuracy of 90% for the provided test dataset.

### 2. Content Relevance & Creativity (25%)

The model should logically match the detected emotion and the creativity of the recommendations is evaluated.

### 3. Code Quality (20%)

The code should be as readable, well-commented as possible and should not be too convoluted.

### 4. User Experience & Personalization (15%)

### 5. Innovation and Technological Relevance (15%)
### RULES

- You cannot use any python module that is not already included in python 3.10

## Submission

To complete the challenge, use [this form](https://docs.google.com/forms/d/e/1FAIpQLSeLD5LKu4fK-r2gTlt9g0Arhz3uliR68bAQum--fsiQDcOATg/viewform?usp=sf_link) to submit a `.py` file containing your solution.

```

```
