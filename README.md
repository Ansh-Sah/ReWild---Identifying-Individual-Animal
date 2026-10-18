# ReWild — Identifying Individual Animals

**AI-powered wildlife re-identification using Machine Learning and Computer Vision**

ReWild is a wildlife identification project designed to identify individual animals from images. It aims to recognize the same animal across different photographs, even when the viewing angle, lighting, distance, or image quality changes.

Unlike basic animal classification, which identifies an animal's species, ReWild focuses on distinguishing individual animals within a species.

## Project Objectives

- Identify individual animals from uploaded images.
- Compare animal images with available reference images or datasets.
- Generate visual features (embeddings) to measure image similarity.
- Support wildlife monitoring, conservation research, and animal tracking.
- Explore the use of AI to reduce the need for invasive animal identification methods.

## Technology Stack

### Frontend
- React
- JavaScript
- HTML and CSS
- Image upload interface

### Backend
- Python
- API-based communication between the frontend and AI model

### Machine Learning
- PyTorch
- Computer Vision
- Deep Learning
- Image embeddings and similarity-based matching

*The final model architecture, dataset configuration, and inference pipeline depend on the implementation used in the project.*

## Project Structure

```text
ReWild/
├── WildTrack/
│   ├── public/
│   ├── src/
│   ├── package.json
│   └── README.md
│
├── tiger-identification/
│   └── backend/
│
├── .gitignore
└── README.md
```

- **WildTrack:** Frontend application for interacting with the wildlife identification system.
- **tiger-identification/backend:** Python backend and machine learning implementation.
- **README.md:** Main project documentation.

## How It Works

1. **Image Upload:** The user uploads a wildlife photograph through the frontend.
2. **Image Processing:** The backend prepares the image for the machine learning model.
3. **Feature Extraction:** The model extracts visual features from the image.
4. **Similarity Matching:** The extracted features are compared against available reference images or stored embeddings.
5. **Identification Result:** The system returns the best available match or indicates that the identity is unknown, depending on the implemented matching logic.

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/Ansh-Sah/ReWild---Identifying-Individual-Animal.git
cd ReWild---Identifying-Individual-Animal
```

### 2. Run the Frontend

```bash
cd WildTrack
npm install
npm run dev
```

Open the local URL displayed in the terminal.

### 3. Run the Backend

Open another terminal:

```bash
cd tiger-identification/backend
```

Install the dependencies listed in the backend's `requirements.txt`, if provided:

```bash
pip install -r requirements.txt
```

Start the backend using the entry-point command specified by the project, such as `python app.py` or `uvicorn main:app --reload`, depending on the framework and file structure.

**Note:** The frontend and backend must be configured to communicate through the correct API URL. Model weights, datasets, and other required assets may need to be downloaded or configured separately.

## Applications

- Wildlife conservation and biodiversity monitoring
- Individual animal tracking
- Wildlife research and field studies
- Camera-trap image analysis
- AI-assisted animal population monitoring

## Team Contributions

### Frontend Development
- **Sarvesh Chaudhari** — Frontend development
- **Upen Kamble** — Frontend development

### Backend and Machine Learning
- **Ansh Kumar** (me) — Backend development, machine learning model implementation, and animal re-identification logic

## Project Status

ReWild is a work in progress. Its identification accuracy and supported species depend on the model, training data, reference images, and evaluation process. A successful similarity match should not automatically be treated as a verified animal identity.

## Future Improvements

- Support for multiple wildlife species
- Improved re-identification accuracy under different lighting and viewing conditions
- Database integration for storing animal identities and image embeddings
- Live camera and camera-trap integration
- Cloud deployment and scalable inference
- Performance evaluation using suitable wildlife re-identification metrics

## License

A license has not yet been specified. Please check the repository for licensing information before reusing or distributing the project.

---

**ReWild — AI for Wildlife Conservation**

*Building technology to help recognize and protect individual animals.*
