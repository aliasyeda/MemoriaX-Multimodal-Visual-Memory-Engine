

# MemoriaX: Multimodal Visual Memory Engine

## Overview

MemoriaX is an AI-powered multimodal visual memory system designed to organize, understand, and retrieve information from egocentric videos using natural language.

Unlike traditional video search systems that rely on filenames or timestamps, MemoriaX converts visual content into semantic memories, allowing users to search videos using natural language such as:

- Find the cooking scene.
- Show me the hiking video.
- Where is someone working on a laptop?
- Find the breakfast preparation.

The system combines computer vision, image captioning, semantic embeddings, and vector databases to create a searchable visual memory.

---

# Features

- Multi-video support
- Egocentric video processing
- Automatic frame extraction
- AI-generated scene descriptions
- Semantic embedding generation
- Natural language video search
- Vector database memory storage
- Visual memory retrieval

---

# Project Pipeline

Videos

↓

OpenCV Frame Extraction

↓

BLIP Image Captioning

↓

BGE Embedding Generation

↓

ChromaDB Vector Storage

↓

Natural Language Query

↓

Semantic Retrieval

↓

Relevant Frame Display

---

# Technologies Used

- Python
- OpenCV
- Hugging Face Transformers
- BLIP Image Captioning
- Sentence Transformers
- BAAI BGE Small Embedding Model
- ChromaDB
- Pillow (PIL)
- NumPy
- Google Colab
- Matplotlib
- tqdm

---

# Workflow

## Step 1

Multiple egocentric videos are uploaded into the system.

Examples include:

- Breakfast preparation
- Tomato garlic rice cooking
- Natural juice preparation
- Laptop working
- Walking and hiking

---

## Step 2

Representative frames are extracted every few seconds using OpenCV.

This significantly reduces redundancy while preserving important visual information.

---

## Step 3

Each frame is processed using the BLIP Image Captioning model.

Example captions include:

- A person preparing breakfast.
- A blender containing strawberries.
- A person walking outdoors.
- Someone working on a laptop.

---

## Step 4

Each caption is converted into a semantic embedding using the BAAI BGE embedding model.

These embeddings capture the semantic meaning of the scene.

---

## Step 5

Embeddings together with frame metadata are stored inside ChromaDB.

Stored metadata includes:

- Video Name
- Frame Name
- Timestamp
- Caption

---

## Step 6

The user enters a natural language query.

Example:

Find the cooking scene.

The system converts the query into an embedding and searches the vector database.

The most semantically similar memories are retrieved and displayed.

---

# Example Queries

Find the breakfast preparation.

Show the hiking scene.

Find the laptop working video.

Show me juice preparation.

Locate the cooking activity.

---

# Example Output

Query:

Find the cooking scene.

Retrieved Result:

Video:
Tomato Garlic Rice

Timestamp:
17.6 seconds

Caption:
A person is preparing tomato garlic rice in a frying pan.

---

# Tech Stack

| Technology | Purpose |
|------------|---------|
| OpenCV | Frame extraction |
| BLIP | Image caption generation |
| BAAI BGE | Semantic embedding generation |
| Sentence Transformers | Text embedding framework |
| ChromaDB | Vector memory database |
| Hugging Face | Pretrained AI models |
| Python | Backend implementation |
| Google Colab | Development environment |

---

# Applications

- Egocentric video understanding
- Visual memory systems
- AI-assisted video search
- Personal video organization
- Semantic multimedia retrieval
- Multimodal AI research

---

# Future Improvements

- Video Question Answering
- Temporal event reasoning
- Memory summarization
- Cross-video event linking
- Real-time streaming support
- Long-term visual memory graphs

---

# Skills Demonstrated

- Computer Vision
- Vision-Language Models
- Multimodal AI
- Semantic Search
- Vector Databases
- Image Captioning
- AI Pipelines
- Video Understanding

---

# Project Highlights

- Built an end-to-end multimodal visual memory pipeline.
- Enabled semantic retrieval across multiple egocentric videos.
- Generated AI-based scene descriptions using vision-language models.
- Stored visual memories in a vector database for efficient retrieval.
- Implemented natural language search over video content.

---

# Developed by
# Syeda Alia Samia
