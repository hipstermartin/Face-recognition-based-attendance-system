# Face-recognition-based-attendance-system

This is a project that implements a face recognition system for tracking attendance. The system captures and preprocesses face images, extracts facial features, and performs similarity checks using image processing and OpenCV algorithms. The system achieves an 80% success rate (for 1000 images).

## Requirements

- Python 3.x
- OpenCV
- NumPy
- Pandas

## Installation

Clone the repository:
  ```bash
  git clone https://github.com/[your-username]/Face-recognition-based-attendance-system.git
  ```
Install the required libraries:
  ```bash
    pip install opencv-python numpy pandas
  ```

## Usage

Prepare a dataset of face images in a directory named dataset. Each image should contain only one face and be named according to the person's name (e.g., john.jpg, jane.png, etc.).
Run the extract_embeddings.py script to extract facial features from the images:
```bash
python extract_embeddings.py
```
Run the train_model.py script to train a face recognition model using the extracted features:
```bash
python train_model.py
```
Run the recognize_faces.py script to perform face recognition on a video stream or a set of test images:
```bash
python recognize_faces.py
```
The script will display the recognized faces and save attendance records in a CSV file named attendance.csv.

## Performance

The system achieves an 80% success rate (for 1000 images) in recognizing faces. The performance can be improved by using larger datasets, more advanced feature extraction methods, and fine-tuning the model's hyperparameters.

## Credits

This project was inspired by the FaceNet paper by Florian Schroff, Dmitry Kalenichenko, and James Philbin (https://arxiv.org/abs/1503.03832).

## License

[MIT](https://choosealicense.com/licenses/mit/)
