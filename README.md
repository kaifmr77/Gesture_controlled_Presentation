# ✋ Hand Gesture Controlled Presentation

This project is a **hand gesture-based presentation controller** built with **OpenCV** and **cvzone**.  
It allows you to navigate and annotate presentation slides in real-time using just your hand — no mouse or keyboard required.

---

## 📌 Features

- **Gesture-based slide navigation**  
  - **Left swipe gesture** → Previous slide  
  - **Right swipe gesture** → Next slide  
- **Real-time hand tracking** using `cvzone.HandTrackingModule`
- **Annotation mode**  
  - Draw on slides with your index finger  
  - Remove last annotation with a specific gesture  
- **Picture-in-picture** view  
  - Webcam feed is shown in the corner of the slides
- **Fully offline** — No internet required

---

## 🛠️ Technologies Used

- **Python 3**
- **OpenCV** – For image processing and webcam feed
- **cvzone** – For hand tracking
- **MediaPipe** – Used internally by `cvzone` for landmark detection
- **NumPy** – For data handling and interpolation

---

## 📂 Project Structure

```
📁 HandGesturePresentation
│── main.py              # Main script
│── 📁 Presentation      # Folder containing slide images
│── requirements.txt     # Python dependencies
```

---

## 🚀 How to Run

### 1️⃣ Clone the repository
```bash
git clone https://github.com/your-username/hand-gesture-presentation.git
cd hand-gesture-presentation
```

### 2️⃣ Install dependencies
```bash
pip install -r requirements.txt
```

### 3️⃣ Add your presentation slides  
Place all your `.jpg` or `.png` slide images inside the `Presentation/` folder.  
The files will be loaded in sorted order.

### 4️⃣ Run the application
```bash
python main.py
```

---

## 🎯 Gestures

| Gesture | Action |
|---------|--------|
| **Thumb up** | Next slide |
| **Index finger up** | Start/continue annotation |
| **Index + middle finger up** | Pointer mode (no drawing) |
| **Three fingers up** | Undo last annotation |
| **Thumb right** | Previous slide |

---

## 📌 Requirements

Create a `requirements.txt` with:
```
opencv-python
cvzone
numpy
```

---



---

## 📜 License

This project is licensed under the MIT License — feel free to use and modify.
